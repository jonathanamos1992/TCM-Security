Having threat intelligence is going to set you up for success when it comes to your ability to contextualize threats and incidents and can
give you that more high level or holistic picture of what it means to cosume and develop threat detections to facilitate quicker response.

Threat intelligence - 

A threat is a circumstance or event that has the potenttial to cause harm to a system or organization.
Can originate from a number of different sources. (ex. malware, phishing from different APT groups or denial or service or man-in-the-middle attacks)

Any other unintended event or circumstance that might not be explicitly malicious in nature.(system failure or human error, natural disasters)

Across the board, we know threats are characterized by their ability to affect the Confidentialty, Integrity, Availability of informations and systems.

Threat intelligence is the process of collecting and analyzing and applying information about potential or current attacks that threaten an organization.

This intelligence allows us to make decisions and take proactive measures to protect our assets.

A specific subset of threat intelligence is Cyber Threat Intelligence or CTI.

And CTI focuses on information related to threats in the digital or cyber domain. (cyber attacks, malware, network intrusions)

Collecting and disseminating information about emerging threats or sources of these threats.

Techniques and behaviors of these threats that can give us data about our external threat landscape.
We're looking outwards to all things that might possibly attack us.

Historically, defensive focus was on configurations and hardening. 

As long as we set up correct firewalls and orientation and configured the right rules and deployed the right anti-virus, we could then call ourselves secure.

With threat actors evolving, and attacks becoming more sophisticated, there's an increasing importance on being able to ingest concise, relevant and informative
threat intelligence data that can help support our detection capabilties.

Ultimately, a big goal of threat intelligence in Attribution.

Attribution - Identifying an actor or actors behind a particular attack, we can better understand and map motivations and capabilties and tactics of threat actors. 
which can enhance our defensive measures for not only our organizations but for any organization facing a similar threat.

Objectives:

Identify threat actors, intelligence sources, and the threat-intelligence lifecycle.
We want to recognize our sources of threat intelliengence (open-source, commericial or internal intelligence)

We also want to understand the different stages of threat intelligence process. (collection, analysis, dissemination.)

We want to understand how to identify tactics, techniques and procedures TTPs.

We want to learn about the structure of TTP's and explore how they're used to classify adversaries at a technical and behavioral level to identify threats.

Exploring common threat intelligence frameworks or models or knowledge bases.

Looking at MITRE ATT&CK Framework or Cyber Kill Chain or Pyramid of Pain, all of which help describe the different stages and methodologes of cyber attacks.
Or techniques employed by adversaries and strategies for detecting and mitigating these indicators effectively.

Learn how to describe and detect malware threats using pattern rules. 

Understand malware behavior and characteristics and explore common pattern rules for detecting malware like YARA rules or SIGMA rules.

Deploy, configure and use a threat intelligence platform to collect and analyze security indicators.

Look at threat feeds, and collect and analyze indicators from various sources and see how we can integrate threat intelligence with other security tools and processes.

## Types of Threat Intelligence

Threat Intelligence can broadly be categorized into 4 types.

Stragetic
Tactical
Operational
Technical

Each type serves a unique purpose and provides different insights to enhance an organization's security posture.

Understanding this will not only put you ahead with ability to contextualize incidents and understand threat intelligence as a whole but 
will be able to speak intelligently about how threat actors operate, different stages of an attack, attack methodologies and how can leverage Indicators of Compromise
to improve our SOC's detections.

Intelligence Types:

Starting at highest level:

## Strategic Threat Intelligence:F

ocuses on high-level analysis of trends or risks and potential impacts of cyber threats on an organzation. Will often include information on a threat actors goal or motives 
or capabilites which can help decision makers shape their long-term security strategies. 

Security Policy Documents or research reports or information that targets trends for specific industries or sectors.
There are alot of companies that produce threat reports (ex. Fireeye, Crowdstrike, Mandiant, Red Canary, and others)

As an example, a piece of strategic threat intelligence could be reading through and disseminating intelligence reports that highlight an increase in nation-state cyber espionage activities targeting the financial sector.
As a senior executive for a large bank, this intelligence can be used to define the organziations current threat model and make more informed decisions about where to invest security controls and products
and allocate resources. (ex. maybe the organization invests more in file-integrity monitoring or endpoint detection and response.)

So we can see with strategic intelligence, we're able to shape the long-term security strategy based on findings in report.
(As example. In the report we can learn about the group and technques used and targets theygo after.)

Then we can start to understand ho this might affect us in our organizationa and industry.

## Tactical Threat Intelligence

TTP's
Going to focus on understanding the methods used that adversaries use to conduct attacks.

When it comes to consuming more tactical intelligence, primarily going to be done by security team and anaylysts instead of high level executives and decision makers. 
This type of intelligence is going to give us more insight into attack vectors or insights into how to create and implement detections and implementation strategies.

We're going to get more into detail into specfic threat actors themselves and behaviors.

Types of actions they typically perform or ways and methodologies they go about staging attacks or type of services and infrastructure or exploits they use.

As an example, we could ingest a report that details these specific phishing techniques used by a particular threat group. Including format of email template or ways they construct their malicious URLs.
MAybe they use typosquatting attacks and impersonate domains or only target a certain subset of an organization's employees.

## Operational Intelligence

More timely and in the moment
Provides information on specific or imminent threats to an organizations.

Include details about planned attacks, targets, or timelines.

You can imagine threat hunters and incident response teams leverage operational intelligence wherever possible to prepare for and respond to active or incoming threats.

Helps mobilize teams to take immediate action to prepare and respond. 

Due to it's very nature, it can be a bit difficult to actual get operational intelligence, unless a threat actor or group has really bad opsec. 
Typcially a threat actor or group isn't going to discuss plans or goals over unencrypted or public spaces.  

Likely done these days over a private telegram group or a forum
Can be hard to get access to these.

If trying to source intelligence from a group that practices good opsec, they are going to have controls in place so that anything that leaks is ambiguous or confusing.

As an exmaple, we could come across a discussion about an upcoming Distributed Denial of Service DDoS against an organizations website or servers or
direct threats froma  threat actor an attack is coming.

Maybe we have an insider threat scenario, a disgrunted employee twho's fed up with their job and tweets about how they're going to take down the organization from the inside.
Or leak sensitive data or intellectual property from the organization.

Maybe the employee thought they were safe by tweeting from an "alt" or puppet account, but because of poor operational security, there are 
traces on this account that lead back to their identity.

## Technical Threat Intelligence

More technical in nature

Information about data related to a threat actors tools or infrastructure or technqiues at a more technical level.

May see a lot of Indicators or Compromise like IP's, file hashes, domain names, host and netowrk signatures from malware.

Target audience: Analysts, engineers and threat intelligence specialists. 

Integrating this technical intelligence into security solutions and tools like IDS or firewalls or SIEM solutions to automate threat detections.

(ex. manually creating a rule in SIEM to detect specific actions on an endpoint or manually wrote Snort rules)

Through this intelligence cycle, we can automatically ingest IOC's or behaviors or signatures into our security appliances to automate our threat detection and make sure we are continuously looking for the latest threats.

Organization can subscribe to threat intelligence feeds and continually ingest latest IOC's and perhaps then able to identify and then load up detection mechansims with
with IP addresses or file hases associated with recently discovered malware compared. 

Makes the more much more prepared to detect and handle if targeted.


## Intelligence Lifecycle

Intelligence isn't a binary thing,

we have to plan out our data collection.
Then we have to process, analyze and turn it into meaninigful insights.

Then share out to right individuals and sort of create that feedback loop to continually improve our process.

To cover each one in detail:

When starting with Threat Intelligence Cycle, we want to start with the most important stage which is the Planning (Requirements and Direction).

## Planning

We need to focus on what we want to actually collect and how we can best do that, and we need to set our goals and objectives and key intelligence questions
for our intelligence gathering strategy.

What do we care about? What do we want to spend money and resources on?

ex. A financial institution might want to gather intelligence on threat campaigns targeting customers or employees of financial institutions, or threats that are targeting banking systems.

ex. A manufacturing company could be concerned with collecting intelligence that could pose a threat to their specialized industrial control system equipment.

Goal is to understand relevant methods, like the malware or the actors, what APT's or threat groups and Indicators of Compromise that are associated with these campaigns that could affect the security of our systems.

We also want to think about the supply chain as well, what threats could affect our vendors or anyone up the chain and how this affects the type of intelligence we want to collect.

## Collection

Involves actually gathering relevant data and information from various sources to address intelligence requirements and goals.

We talked about all of the internal data and events we can capture like packet captures, or endpoint logs or EDR or SIEM agents.

Here we're focusing on external data as well.

Wide range of sources (paid and proprietary. )

Different Types of Sources of Intelligence:

Internal Threat Intellgence - Data generated from within an organization from it's own systems and operations. Looking at logs from firewalls or IDS or IPS systems or EDR, anti-virus software, as well as incident reports and lessons learns and post-mortems form past incidents.

Primary benefit of internal threat intelligence: 

1. Readily and continously available, don't have to subscribe or pay for it. 
Kind of an indirect benefit of having this ability over our enviornment.

2. Tailored to our specific envirornment. Type of data ingested is highly relevant.

On the external side:

We have number of different sources of threat intelligence data as well.

First off, open source intelligence or OSINT

OSINT- gathering information from publicly available sources: websites, social media, different forums or published research.

since the information is publically available. OSINT can be a cost-effective way to enhance our threat intelligence.

We ARE going to get a vast amount of data.

NEED to distinguish whatis both ACCURATE and USEFUL.

ex. Monitoring things like the dark web, or different forums or social media. Chatrooms like Telegram channels where cybercriminlas exchange information and or sell exploits plan things like data leaks or plan different attacks, or look at public databases of information relevant to vulnerabilities or malware or information on systems in general.

ex. Common Vulnerabilities and Exposure CVE Database, MalwareBazaar, Virustotal, Cisco Talos, Anyruns.

In regards to open source threat feeds we have things like US CERT - United States Computer Emergency Readiness Team which provides cybersecurity alerts and advisories and different reports on threats affecting the US.

In the UK, there's the National Cybersecurity Center, NSC.

We also have things like the Open Threat Exchange, now owned by AT&T.

And we'll also look at MISP or Malware Information Sharing Platform.

All these can provide insight into emerging threats, or track threat actors and significantly support operational intelligence.

### Commerical Threat Intelligence

Provided by 3rd party vendors who specialize in services usually related to threat intelligence, or network or endpoint detection platforms.

These vendors analyze and collect data from various sources. Like they're own research and honeypots or honeynets or their own solutions, like own data collected from customer systems.

Can provide clients with collected and closed source data collected, closed source data in the form of actionable intelligence. 

ex. Mandiant with their cyber threat intelligence platform or RecordedFuture.

Reason why commercial intelligence can be useful is because it can be tailored to meet specific needs or an organizations and and gives us insights that might not be available through internal or open sources.

Organizations may subscribe to various threat intelligence feeds that can provide real in-time information on known threats and IOCs or different malware signatures and attack patterns that are ready to be ingested into different security tools and detection mechanisms.

Downside is that these services can be costly. Organizations need to evaluate the value and how they're going to use it to justify the costs.

As another intelligence source, we can look at reports and white papers published by cybersecurity vendors and researchers and these can provide analysis of recent threats or attack vectors or tactics and techniques of threat actors. 

Lastly, concept of collaborative intelligence collection and dissemination

Information Sharing and Analysis Centers (ISACs) - nonprofit entities where organization within the same industry share threat intellgience and best practices to each of its members. Membership driven. Membership with an ISAC requires organizations commitment to active participation and sharing. Since this is a collaborative process. Quality of intelligence depends on contribution of its members. 

There are recognized ISACs for a number of different industries.
Several ISACs or critical infrastructure ex. metals and mining, finance, automotive, aviation, electricity, healthcare, real estate, public transportation, etc.

### 















