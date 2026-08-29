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
<img width="873" height="200" alt="image" src="https://github.com/user-attachments/assets/453b47d0-5939-444e-80ae-53d45878e4e7" />


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
<img width="1434" height="1191" alt="image" src="https://github.com/user-attachments/assets/4009b400-0dad-4483-bb14-85193d31b499" />

So let's start out with the Fortigate or Firewall logs.
We'll look in the botsv1 index for these logs

```
index=botsv1 sourcetype=fgt_*
```

Utilizing the wildcard, we can match across all Fortigate ftm logs

<img width="1434" height="1050" alt="image" src="https://github.com/user-attachments/assets/31eedab3-2aa3-4434-927d-bbc2f8dd87e5" />

Since we're getting a lot of events back (3 million and counting) which includes all kinds of network activity, let's narrow the scope of what we're looking for. 

This Scenario is specifically about the suspected compromise of imreallynotbatman.com, so let's include that.

<img width="897" height="75" alt="image" src="https://github.com/user-attachments/assets/b2d14762-f037-4cf8-aac9-90d46d89fe01" />

<img width="845" height="77" alt="image" src="https://github.com/user-attachments/assets/3da309b0-3dea-40a6-be47-5bc95bf409e0" />

### Results 

<img width="1429" height="1197" alt="image" src="https://github.com/user-attachments/assets/99cc4709-a01b-43b9-bca1-08c004db5218" />

Now we can click on an event and see what fields we have.

Since these are firewall logs, we have fields like 'Action' that show if the traffic was allowed or denied.

We can also see things like the URL which shows what the actual URL is on the page that's being access through the firewall.

So there's a few things we can do here. 

-Look at top values for Source IP address.

<img width="1149" height="869" alt="image" src="https://github.com/user-attachments/assets/c45869a1-3ac4-4030-ab13-52c0c82bb353" />

With this we see we only have 2 IP address to look through.

Interesting but not explicitly definitive on its own but can warrant further investigation.

We also see from the percentages that 40.80.148.42 is comprising over 90% of the traffic. 

With the high amount of traffic from a single IP, we could hypothesize that the attacker could have ran a vulnerability scanner.

<img width="940" height="455" alt="image" src="https://github.com/user-attachments/assets/e3d5451a-4b06-42cd-93bc-2f6511627fa6" />



Since this is a firewall, let's look at the available actions within our results.

<img width="1432" height="664" alt="image" src="https://github.com/user-attachments/assets/48af214b-caef-4528-84eb-61fad4edeb68" />

We see Allowed, Blocked, and Deferred

Since we hypothesized that the attacker might have ran some kind of vulnerability scanner, it's a safe bet that some of those packets may have been blocked.

Let's add the "blocked" field to our search.

<img width="1429" height="1219" alt="image" src="https://github.com/user-attachments/assets/6de1e371-3144-4d0a-88a6-7d0c360c1de0" />

### Results

<img width="1425" height="1188" alt="image" src="https://github.com/user-attachments/assets/5ca7f1c2-8fff-4286-bf9f-07d28866e9dd" />

This cut our results down to 4,000 events and when we look in the Source IP field, we only see one result. Again the 40.80.148.42

<img width="1417" height="666" alt="image" src="https://github.com/user-attachments/assets/d9789a32-e2e3-40a1-a35c-c234c05f3f82" />

It seems to be the only IP address getting blocked. Adding suspicion and adding to our hypothesis and adding to our judgement calls.

So while we have 4000 events, let's open up an event and see what we have available to us. 

<img width="1438" height="1184" alt="image" src="https://github.com/user-attachments/assets/4d5a9206-0150-4894-838a-f9768a685668" />

In the attack field, we can see that the action was blocked because it identified a web vulnerability scan from Acunetix software.

Acunetix is a vulnerability scanner similar to Nessus. Can be used to probe an endpoint and find out any vulnerabilities or flaws that can lead to exploits.

Often used for vulnerability management in Governance, Risk Management and Compliance (GRC).
Folks that regularly scan an organization's resource, making sure they're all patched an no major vulnerabilities out in production.

So there's a possibility that this could have been done legitimately and the vulnerability management team didn't tell the sysadmin or SOC to allow that Acunetix traffic through so we see a bunch of denied traffic.

But it seems fair to say this could be attacker scanning the website.

Under the attack ID field, we can Google the number. 

<img width="1430" height="1146" alt="image" src="https://github.com/user-attachments/assets/54592e65-6e3a-4e8a-85fb-35b0efb6249a" />

<img width="1412" height="1179" alt="image" src="https://github.com/user-attachments/assets/a98b081d-93d8-4828-94d0-765d014d0215" />

<img width="1438" height="1254" alt="image" src="https://github.com/user-attachments/assets/a8a6d4f4-d430-4e82-8ac1-356034daccc8" />

So we can see this type of alert of drop action, occurs when the Fortigate firewall detects an attempted scan from the Acunetix vulnerability scanner.

From here we have enough information to answer our first question.

## Question 1

<img width="880" height="685" alt="image" src="https://github.com/user-attachments/assets/8cb7a10b-f7d4-4e11-858a-86a03168f769" />




















