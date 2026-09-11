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



































