* Every analyst is going to approach an investigation differently.
* Following a general process, questions to ask, etc.

<img width="1439" height="1249" alt="image" src="https://github.com/user-attachments/assets/6f6d6f3f-7dd0-4bb1-a8fd-48b0b6786fda" />

Choose scenario 1
<img width="1173" height="1132" alt="image" src="https://github.com/user-attachments/assets/531d55cb-d0b4-400f-b762-c42e6bd45ef0" />

We need to know what data or indexes are available to us, which will determine searches and correlation capability and overall strategy.

When we encounter a new Splunk instance or data we're not familiar with, we want to understand what indexes have been indexed in Splunk and what kind of sourcetypes we have available as well.

Index - where the data is stored

Sourcetype = what kind of data it is and how Splunk should interpret it.

<img width="866" height="596" alt="image" src="https://github.com/user-attachments/assets/0952aa23-199d-4b74-a1db-45ac39686375" />

We can use the following event count and metadata commands to list out all of the indexes, or hosts and sources and sourcetypes within our system.

 ### Generating Commands

 <img width="902" height="495" alt="image" src="https://github.com/user-attachments/assets/ed4fc85a-2c93-488e-814d-ccbb5cf1ca3a" />

```
| eventcount summarize=false index=*
```

eventcount command will count events per index.

summarize set to false will ensure we don't miss any information

Wildcard * will pull every index.

<img width="864" height="1246" alt="image" src="https://github.com/user-attachments/assets/330acc81-e353-481e-81da-02b6be1d3d85" />

<img width="1435" height="684" alt="image" src="https://github.com/user-attachments/assets/f6879ecc-03f3-4558-9b9f-f97348a4f245" />

Now for the sourcetype.

We have botsv1 index but in this simulated network we have logs flowing in from a number different sources, like endpoints, servers, networking equipment and security appliances.
So let's list out the scope of what event sources or logs we have to work with and correlate.

```
| metadata type=sourcetypes
| fields sourcetype
```

The Metadata command asks Splunk for information about the data Splunk knows about.
<img width="1424" height="927" alt="image" src="https://github.com/user-attachments/assets/64be143e-eb86-45de-a82e-41f07d953596" />

Then `fields sourcetype' takes those results and says "Only show me the sourcetype field"

From the results we see we're getting 23 different sourcetypes

These source types can provide different endpoint visibility.

ftg - Fortigate firewall
ftg-utm - Fortigate Unified Threat Management logs - will give us information about intrusion detection and prevetion as well as web-filtering,.

### For website defacement, this can be useful

### Always put the visibility of what we have into the context of what we're investigating. This prevents going down unnecessary rabbit holes.

<img width="744" height="317" alt="image" src="https://github.com/user-attachments/assets/a9f9cb5d-b58c-416d-8922-41b86567ed70" />

We also see stream data which usually means PCAP data or events going over the wire or network.

We also see Suricata: widely-used, open-sourced IDS
Can inspect packets and create alerts based on signatures.

## Questions

<img width="781" height="739" alt="image" src="https://github.com/user-attachments/assets/76c81e64-66e8-45fa-8ba4-6c4048f115aa" />

When we think about the stages of an attack, they often need to start with reconnaissance to discover information about the target, like what type of web server is running, version,
applications, employees or users that can be enumerated, cross-referencing that with any vulnerabilities that can be used against the systems.

So when we're thinking of identifying things like reconnaissance against a web-server, we want to think about what source-types we have available to us.
And what types of those would contain relevant data, an indicators like a scan.

So if they're scanning a website that means their sending in inbound packets towards a web-server, meaning it's going to be a network-based event.
So if we have some sort of firewall in place in front of a web server, or an IDS or IPS sitting in between or on endpoint,
Well these are appliances that may be able to detect and block the activity. 

<img width="1633" height="1070" alt="image" src="https://github.com/user-attachments/assets/d1400bc0-112d-4359-8914-88c132442214" />

### We can likely find the answer using any of these methods.
Every analyst can approach something differently and still achieve the same result.

### Starting Search

First we need to search for the appropriate time-range. 

From the incident briefing document, we see the incident took place in August of 2016. 

<img width="1433" height="1163" alt="image" src="https://github.com/user-attachments/assets/1da1c69a-749c-4b36-aab1-5937469f6305" />





































































