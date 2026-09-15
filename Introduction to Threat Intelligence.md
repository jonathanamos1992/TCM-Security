Having threat intelligence is going to set you up for success when it comes to your ability to contextualize threats and incidents and can
give you that more high level or holistic picture of what it means to consume and develop threat detections to facilitate quicker response.

Threat intelligence - 

A threat is a circumstance or event that has the potential to cause harm to a system or organization.
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

<img width="925" height="2258" alt="image" src="https://github.com/user-attachments/assets/e248c211-eb88-4586-beca-9070c205f5ca" />


Each type serves a unique purpose and provides different insights to enhance an organization's security posture.

Understanding this will not only put you ahead with ability to contextualize incidents and understand threat intelligence as a whole but 
will be able to speak intelligently about how threat actors operate, different stages of an attack, attack methodologies and how can leverage Indicators of Compromise
to improve our SOC's detections.

Intelligence Types:

Starting at highest level:

## Strategic Threat Intelligence:

Focuses on high-level analysis of trends or risks and potential impacts of cyber threats on an organzation. Will often include information on a threat actors goal or motives 
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

Internal Threat Intellgence - Data generated from within an organization from it's own systems and operations. Looking at logs from firewalls or IDS or IPS systems or EDR, anti-virus software, as well as incident reports and lessons learned and post-mortems form past incidents.

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

After we've collected all of the data, we enter the processing phase where data can be analyzed and turned into actionable intelligence. 
So we might need to clean up and normalize the structure of raw data to make it suitable for analysis.

We might need to parse through events or logs or extract relevant fields depending on the source.

Purpose here is to prepare the data for in-depth analysis, ensure it's accurate and in a format can be easily interpreted. 

This leads us to the next step.

### Analysis

Where the processed data is examined to uncover patterns and trends as well as actionable insights.
This can use techniques like pattern recognition, statistical models or correlation methods.
Or could involve comparing the data against known threat indicators to validate any findings.

Goal is to to provide intelligence that is relevant and actionable, and attack vectors that can information decision making and response strategies.

### Dissimenation

Once we have actionable intelligence, we need to distribute it and communicate it to stakeholders.

In a concise and timely manner.

May involve things like intelligence briefings to different departments or teams, or through various reports that are sent out to relevant parties in ways that are tailored to the needs of the audience.

Effective dissemination ensures that the intelligence is actionable, and decision makers can prioritize, spend resources effectively. 
Or security teams can implement specific controls or detection methods as they relate to intelligence that was gathered.

Now with any good lifecycle, we generate a feedback loop to ensure it's ever evolving and improving.

### Feedback

Crucial for refining and improving the intelligence lifecycle as a whole.

By reviewing and evaluation the effectiveness of all of the intelligence that was produced and actions taken as a result. 

We can gauge how effective our threat intelligence strategy is.

We can measure metrics like the relevance, accuracy and timelines of the provided intelligence and use that to assess how well our initial objectives that we set out during the planning stages were met and whether there are any areas for improvement. 

### Diamond Model of Intrusion Analysis

<img width="1270" height="679" alt="image" src="https://github.com/user-attachments/assets/087ab66d-4383-4448-b9fd-0a172583243a" />


Establishes the basic atomic element for any intrusion activity, which is the event.

Composed of four core features.

Adversary
Capability
Infrastructure
Victim

Intends to provide more structured approach to analyzing a visualizing the relationships between different components of a cyber intrusion or attack.

Four components are related and innately connected to each other. 

Big purpose of the Diamond Model is to be able to map out these four quadrants and achieve attribution or identify threat actor or group responsible for cyber incidents.

Very flexibile framework we can apply to attacks of all sizes, or industries or sophistication.

So with attribution we first have the adversary.

### Adversary - Individual or group that's responsible for the intrusion.

Can range from independent hackers or organized criminal groups to nation states.
When thinking about the adversary, we aim to answer questions like where is the origin of the attack.

(i.e. where is the adversary from, from which part of the world geographically, who are the individuals or groups beind the intrusion, are they sponsored by some type of organization or entity? 

Motivations? Are they hacktivists where attack is driven by ideological reasons or cyber-criminal looking for financial gain, or nation-state actors fueled by geo-political interests.

Often not going to know answers right away and will have to use other parts of Diamond Model and fill in gaps and interconnections before we can pin-point the adversary.

So first feature (adversary) will often be unknown, especially at the time of discovery. 

### capability:

Adversary is the actor or organization responsible for utilizing a capability against the victim to achieve their intent. 

When we think about interconnection of different features within the diamond model, it can be helpful to include verbs to describe actions and processes between them. 

<img width="1265" height="684" alt="image" src="https://github.com/user-attachments/assets/07ef58f7-9d0c-42e9-accb-ccd6537b3ac2" />

Capabilities are things that are developed and used by adversaries during an attack.

Often here we're thinking about TTP's, different tools and methodologies, behavior and overall techniques the attacker uses. 
Also going to include the adversaries sophistication level.

How capable are they?
How good is their reconnaissance?
What tools do they use for reconnaissance or delivery or exploitation?

Do they develop their own tools?

How good is their malware at getting around detections or evading antivirus?

Do they have possession of any zero days?

Next we can cut through the diamond and land at infrastructure.

### Infrastructure

You can see here that as adversaries develop and use various capabilities, these capabilites and TTP's get deployed through various infrastructure.

Infrastructure refers to all of the different resources and systems leveraged by the adversary to facilitate their attack.
Technical backbone and infrastructure of their operations.

(i.e. IP addresses, domain names, email addresses, USB devices, command and control servers, any other technical element used to support and manage the intrusion.)

Means that the adversary uses to deliver a capability or maintain control of their capabilities such as a command and control scenario
and complete actions on objectives from the victim.
(i.e. exfiltrate data or move laterally to compromise further systems).

Any of this infrastructure can be referred to as Type 1 Infrastructure or First Party Infrastructure that's owned and controlled by the adversary themselves. 

With Type 1 infrastructure, we can infer some type of physical proximity to infrastructure itself such as physical servers or endpoints.
But more often than not we're going to run into Type 2 infrastructure. 

Type 2 infrastructure - controlled by an intermediary, whether knowing or unknowingly.

Typically this is the type of infrastructure that the victim will see as their adversary, even if it might be hosted or operated and owned by unlreated parties.

So we get more obfuscation and difficulty when it comes to geographic origin and attribution.
(i.e. zombies within a botnet or malicious domains hosted by a non-affiliated registrar, compromised email accounts that are used to stage phishing campaigns, systems like command and control servers or malware staging servers that are spun up in cloud enviornments, which makes attribution more difficult.

Say we investigate an IP address and it ends up being owned by Microsoft or Amazon...Are they the adversary? Likely not.)

<img width="966" height="977" alt="image" src="https://github.com/user-attachments/assets/9e1026fd-da61-490c-a8e0-8cbe47bc5719" />

https://www.microsoft.com/en-us/security/blog/2024/08/28/peach-sandstorm-deploys-new-custom-tickler-malware-in-long-running-intelligence-gathering-operations/?utm_source=chatgpt.com

### Victim

Target of the adversary
Adversary uses its capabilities and infrastructure to connect to and exploit the target and carry out the attack

Can be an individual, or system or organization.

Model is flexible...can be a person, an entire organization, a email account, an IP address or domain.

Model likes to make a distinction between what is referred to as victim persona and victim assets.

Victim Persona - People and organizations that are targeted in a cyber attack
(i.e. key personnel in an organization or specific industries or sectors)

Victim Assets = Actual components of targets digital presence that adversary aims to exploit.
(i.e. systems, actual software or hardware, networks or email addresses, servers or hosts or IP addresses.)

Actual endpoints themselves.

### Case Study: Stuxnet

Highly sophisticated worm discovered in June 2010
Designed to target Industrial Control Systems, specifically ones used in nuclear facilities

Created to sabotage Iran's nuclear program by targeting it's uranium enrichment facilities.
Aimed at Siemen's Programmable Logic Controllers that controlled actual centrifuges used in uranium enrichment.

<img width="1274" height="716" alt="image" src="https://github.com/user-attachments/assets/89362b98-bf8a-4e71-a544-d1805912bd72" />

Walking through the Diamond Model

<img width="1269" height="692" alt="image" src="https://github.com/user-attachments/assets/fa37a030-79a0-4d6b-b628-65835a79c6b1" />

### Adversary

We didn't have enough information to attribute to the identity of the adversary.

#### Capability

<img width="1333" height="729" alt="image" src="https://github.com/user-attachments/assets/027e2eef-f5ed-47b3-a324-5ec857f606a3" />


A number of Zero Day Exploits that were chained together to make this attack happen. 
Four of them related to Windows

We know there was a link file which automated execution of the propagated worm copies.
And a root kit installed as well in both user and kernel mode.

To install kernel-mode root kit, used digitally-signed certificate drivers that used private-key certificates stolen from two well-known Taiwanese device manufactures. 

Once in control of PLCs, Stuxnet varied rotation speeds of centrifuges while in operation. While doing this, ran at unsafe speeds until they failed. 

<img width="1233" height="692" alt="image" src="https://github.com/user-attachments/assets/86f6944e-e7b4-4f14-a28d-522c2e9b4b9e" />

##### Now we have adversary that developed capabilities which were deployed through the infrastructure.

#### Infrastructure 
On the infrastructure side, we can think about the attack infrastructure and the propagation or delivery methods of the attack.

Stuxnet worm was initial delivered through an infected USB drive.

This is because the physical facility where uranium-enrichment was taking place was known to be air-gapped.

Once on the systems, the worm was able to spread quickly from machine to machine on the internal network. 

#### Victim

Victim assets - Siemens Step 7 software of the Programmable Logic Controllers
Victim Persona - Iran and its nuclear enrichment facility

Unintended secondary victims - during its spread Stuxnet infected other systems and escaped facility, likely on someone's laptop and then connected to the outside internet and spread in public. 

### Analysis

We don't know the adversary but can start using the model to sort of narrow down who the potential adversaries could be.

We can ask qeustions like:

"who would have the ability or capability to research and chain together 4 Zero Day Vulnerabilities?

Who would be able to develop these exploits specific to Siemens Industrial Control Systems

Description alone should make it clear that Stuxnet was part of a high-level sabotage operation by a high-funded organization like a nation state.

This eliminates large number of potential adversaries and we can focus on high-funded groups or insiders with socio-political motivations.

##### We can think about motivations themselves

Who would want tot impede Iran's nuclear program and prevent them from developing nuclear weapons?

We can start thinking about who are the enemies of Iran?

Speculation early on about government-backed hacking groups form China and Russia

China was in a space race with India at the time, India used the same Siemens controller equipment within some of their satellites.
Maybe that's who China was targeting. In fact, one of the Indian satellites using Siemen technology with power glitch around the same time.
With that there was a lot of speculation that Stuxnet might have attempted to affect the space race between China and India.

Also theories around Germany as well as that's where Siemens was headquarted.

Also some files in Stuxnet as well that hinted to Israel's involvement. 

While there are competing theories, using the diamond model helped pinpoint who has this capability and who would be able to deploy it with this infrastructure, and who would have the motivation.

These are the ways in which we can start to formulate different hypotheses on how we can develop our adversary. 
Not always a quick process, can take months or years to pinpoint. 

Turned out to be US and Israel in a polital effort to deter Iran's nuclear program.

Now we can start moving through the different actions and interconnections within the Diamond Model and see how everything works. 

<img width="1327" height="712" alt="image" src="https://github.com/user-attachments/assets/b32d6ea4-c1ee-4b11-860a-7a2daa1a7999" />

Adversary (US and Israel) developed advanced technical capabilities in that they created a worm that exploited zero day vulnerabilities and used stolen certificates and had complex payloads specific to industrial control systems equipment.

When we think about the link between Adversary and infrastructure, the capabilities the adversary developed were deployed through physical air-gapped facility with infected USB drives, ensuring worm could propagate and remain undetected.

When we think about infrastructure and victim. Worms deployment through USB drives and network shares allowed it to penetrate and spread within the facility's network and reaching the PLCs and executing its sabotage. 

When we thinking about capability exploiting the victim, the zero day and sophisticated malware that was deployed was used to exploit the centrifuges and render them inoperable. 

Learning about frameworks and models, we are able to have a more structured approached to highlighting the relationships between adversary and capabilities, infrastructure and victim, we can better understand complex threat actors and their capabilities, which ultimately leads to attribution and also helps us predict and prevent future incidents.

[Using Honeynets and Diamond Model for ICS Threat Analysis](https://infocon.org/mirrors/vx%20underground%20-%202025%20June/APTs/2016/2016.05.09%20-%20Using%20Honeynets%20and%20the%20Diamond%20Model%20for%20ICS%20Threat%20Analysis/Paper/Using%20honeypots%20%26%20diamond%20model%20for%20ics%20threat%20analysis.pdf)

#### Now we can move onto discussing the different stages of a cyber attack

## Cyber Kill Chain

The most well known model in this domain is the Cyber Kill Chain developed by Lockheed Martin,


*Picture of Cyber Kill Chain* 

Based off the military concept, parallels to be made in attacking and defending both physically and kinetically in a cyber landscape.

Cyber Kill Chain is a conceptual framework that is used to break down the different stages of an attack. 

Serves as a guide for organizations to understand, detect and defend what adversaries are doing by detailing the phase of a typical attack.

By understanding each phase of an attack through the lens of the cyber kill chain, it can help us an analysts and organizations to develop more comprehensive security strategies. 

This brings us to the concept of Defense in Depth

We can develop our security strategy to intercept an attack at multiple points. 

Some may argue that the Cyber Kill Chain is too rigid or doesn't account for certain types of attacks.
(i.e. some attacks don't follow the chain to the T.)
Maybe, but we can also apply some common sense as well.

Learning a framework like the Cyber Kill Chain allows us to systematically understand the potential phases of an attack, even if what we see in the wild doesn't match precisely.

# 7 Stages of the Cyber Kill Chain

### Reconnaissance

During this phase an attacker is going to gather information about their target and the information that they gather during this phase will help them plan out the proceding phases of an attack.

Long phase and sometimes the longest phase of an attack and sometimes the longest phase in the kill chain.

We can compare this to a military operation with the longest part of planning any type of attack is going to require a lot of extensive research of a target.

i.e. 
Where's the best place to land or attack from?
What's the best time to attack?
What do the enemy's defenses look like?
Are we going in loud or tactical?

The same concept can be said about a hack or cyberattack.

A threat actor needs to understand the lay of the land and research the target accordingly.

This might include reasearching publicly available data or performing OSINT. 
An attacker could be collecting as much passive information as they can.

Whereas they don't actually perform any active scanning or probes, just seeing what information can be gathered from a typical non-assuming perspective.

On the OSINT side, this could be personal identifiers about employees, email addresses, or full names, phone numbers or even more contextual information such as interests or favorite teams. 

These can all be used to create word lists to be able to brute force credentials later on.

Sometimes it doesn't even need to be done.
If an attacker can get thier hands on previous data or credential breach, they might be able to figure out a users credentials this way, without ever having to interact with them if the user is using their password anywhere else.

This can also include active techniques as well, such as scanning the target's actual systems or networks or using social engineering techniques to identify potential vulnerabilities or attack methods.

Maybe an attacker is running NMAP on a target's web servers to see what services or languages or stack that its running.

Or looking for Whois or Shodan to map out an ip space to see what ports and services are open.

Maybe they're running vulnerabilities scans or enumerating web pafes or directories or sub-domains.

Reconnaisance phishing emails can be used by an attacker to verify if a user's mailbox exists or suspectible to opening an external email, or if they can get a response.

We also talked about tracking pixels which can help an attacker fingerprint an organizations email server or profile their target at the endpoint level as well.

And enumerating things like the email client software or the operating system version or web browser.

At a physical level, maybe an attacker is tailgating an employee to map out security camera locations or alarms.

Maybe their talking to employees in the lobby or outback, trying to secretly get information to stage a future attack.

Or maybe looking through disposed material known as dumpster diving, to see if any sensitive data has been thrown out unknowingly.

Information will help an attacker tailor their approach and their future weaponization and delivery methods to maximize their chances of success later on.

This all leads us into the next phase, weaponization

### Weaponization

Where an attacker actually goes about developing their malware or malicious payloads designed to exploit any identified vulnerabilities or attack vectors discovered during their reconnaissance. 

Often this stage is going to involve an attacker combining their malware or exploit into a deliverable payload, such as a phishing email attachment or a malicious website, or even other client-side attacks like a benign looking Word or Excel file that actually has embedded malware scripts inside.

We looked at examples of these types of attacks as well.

Weaponization phase can also be things like standard service exploit like some of the web-based attacks that can lead to things like remote code execution, or things like a buffer overflow against a network service.

Often this isn't as simple as pulling an exploit off of ExploitDB or Github.

Often if an attacker goes the route, the exploit needs to be heavily modified or they'll create their own entirely.

Or pay money for an exploit that will suit their needs. 

Or it may involve chaining multiple Zero Days together.

When talking about the market of Zero Days, could be multiple millions of dollars for an exploit.
Highly funded groups will pay for it.

That's because developing a reliable payload that can get around things like patches or detections and different security controls or antivirus can be quite an involved and expensive process.

Once the exploits and payloads have been acquired or developed, the next stage in the Kill Chain is the Delivery phase.

### Delivery

Actual way for the weaponized payload to actually transfer and make it to the target, whether it be a server-side attack against a network server or a client-side attack against a user.

This is where all of the information gathered during the recon phase come into play, the more information an attacker has about its target and system, the more avenues for delivery they will have.

Could be as simple as having more email addresses they can phish, or more enumerated services they can connect to. 
Most common methods of delivery will be things like phishing emails with malicious attachments, or links or URLS, or malicious USBs that get dropped around, or drive-by downloads on the compromised websites, or direct exploitation of any web or network vulnerabilties.

We can see how client-side attacks are more popular because getting a phishing email onto an end-users endbox is a lot easier to do at scale. Also easier to evade traditional permieter controls if an email is coming through a 3rd party email service.

So return on investment for an attacker is much higher.
Still plenty ways to defend agaisnt phishing and social engineering attacks.

Typically easier to exploit humans than it is to exploit a server or technology.

Another significant method of delivery is through supply chain attacks.

Where adversaries compromise a third party vendor or supplier that provides software or services to the target organization.

By inserting their malware into legitimate software upstream, an attacker may be able to infiltrate indirectly.

All the previous steps lead up to the next stage, Exploitation.

### Exploitation

All the legwork put in to make the attack comes together.

Where the already delivered malicious payload is executed on the target system, or interacted with on the endpoint.
Involves the entire exploit chain as well.

If the attack involves chaining multiple exploits together, for example, exploiting a LFI vulnerabiltiy on a server to include a log file, and then poisoing that log file with a malicious user agent that executes php code, essentially giving the attacker remote code execution.

Then using that web shell to execute a reverse shell back to the attacker.

Many different examples here because this stage can involve many things like running or executing malicious code, or VBA scripts within a document or running a malware executable or exploiting a software vulnerability or buffer overflow executing to gain remote code execution on a server, or just by using stolen credentials from a phish to gain access to an account or system.

Exploitation phase basically marks point where attacker gains control over a system or gets that initial foothold.

### Installation

Back when we were looking at endpoint section, we were looking at alot of different mechanisms that were installed on endpoints.
These were persistence mechanisms, which are a big part of the Installation phase.

Once an attacker exploits a target and gains that initial shell or intial access, they typically want to upgrade their newfound access into something more stable and more reliable as they plan to do what they need to do on the system or keep their long term access.

During this phase the attacker may install additional malware like a backdoor or a rootkit on the target or victim system, to maintain persistent access.

This can be things like auto-start implants that we were looking at earlier, so those run entries in the registry that can point to malware. We can see installed services or scheduled tasks.

Often we'll see things here like DLL injections where an attacker injects a malicious dynamic link library into a running process or things like memory injection which can execute malware within the memory space of a legitimate process, without writing any code or files to disk.

Anytime we start venturing into fileless or memory-based malware, this makes detection a lot more difficult for traditional security solutions which typically monitor for files on disk.

Ultimate goal of installation here is to ensure that the attacker can return to the compromised system, even if the initial access or vulnerability is patched or the system is rebooted. 

So we're almost at the end of the chain here and we can think about how the attacker did their recon.

They did all their reconnaissance and learned about the target
Wrote or acquired their malware,
Delivered it to the target
Exploited it
Made sure they have stable long-term access or persistence on the system.

What next?

Typically establish what is known as command and control or C2.

Communication channel between the compromised system and the attackers infrastructure.

Setting up this channel allows the attacker to send commands and recieve data and in general just control the infected system remotely, without having to re-exploit the system every time.

When we're thinking about detections at this stage, alot of this is going to be network-based. 

Command and control servers are often established using known and trusted protocols like HTTP or HTTPS or DNS with DNS Tunneling.

While we've demonstrated malware in the past that has easy to identify ports like 4444, that was only to understand the principles. 

Real attackers won't be obvious.

At a high level we can think about abnormal traffic patterns.
Looking at things like session length and identify any super long or persistent connections that deviate from the norm.

We can look at communication patterns at attackers C2 channel that sends a keep-alive or beacon at known frequencies.

(i.e. Attackers C2 channel sends a keep alive or a beacon sending 100 bytes every 30 minutes until the attacker gives an order to run a command on the system.

A good attacker that cares about their opsec will implement things like "jitter" to any of their keep alives or beacons so its not exactly the same size everytime.

We can do things like statistical analysis that will average out the sizes and when we put it on a graph, it will look pretty consistent.

When we look at the amount of packets transferred over, in cases of exfiltration or look at things like a high number of dns queries to the same domains.

Maybe some sort of dns tunneling or dns exfiltration.

Ultimately the goal of C2 or Command and Control is so the attacker can orchestrate their actions and potentially move laterally within the network as well.

This brings us to the most important stage of the Cyber Kill Chain - reason why attacker did all the work.

Where all the previous steps converge and where attacker can go about main objectives or ultimate goal for the target.

### Actions on Objectives

Can vary widely depending on the purpose of the attack or attacker, or victim.
We can think about the actual motivations for the attack itself.

Often see things like credentialharvesting - dumping credentials from the compromised system or finding them hardcoded somewhere on the device.
Then using credentials to pivot around the network, spray them around or use them to stage future attacks and start the Kill Chain over again.

Can also include things like Data Exfiltration (i.e. stealiong databases or customer information or financial details, intellectual property or stealing sensitive documents from emails, network shares or desktops.)

If attacker is more malicious, can destroy data, or take down systems or servers or deface them in some way.

If attacker is more financially motivated, ransomware.

Actions on objectives can vary on the attackers motives.

Financial gain
espionage,
hacktivism,
disruption
competitive advantage

While its a rigid structure, the Cyber Kill Chain gives us a more holistic and comprehensive understanding of the lifecycle of a typical cyber attack.

Reason why we do this as SOC analysts is because organizations can use this model to develop more targeted defenses in-depth, to address each stage of the kill chain and improve overall ability to detect and mitigate and respond where ever an attacker might be during their execution.

(i.e. security measures like network monitoring or intrusion detection systems or endpoint protection or even just user education can all be aligned within the different stages of the cyber kill chain to create a more comprehensive defense in depth strategy.

Further reading:

Unified Kill Chain - Integrates and expands on elements from the Lockheed Martin Cyber Kill Chain and the MITRE ATT&CK Framework and other models to provide a more unified perspective on adversarial behavior.

Aslo helps address some of the drawbacks of the Cyber Kill Chain suhch as being too rigid and doesn't always map to certain attacks. 

(Unified Kill Chain)[https://www.unifiedkillchain.com/assets/The-Unified-Kill-Chain.pdf]

### Pyramid of Pain

Drives home the concept of what Indicators of Compromise or IOC's really are.

As we've been working our way down to mapping out threat actors and ultimately their motivations and ultimately the chain of their attacks, well the pyramid of pain allows us to look into the actual internals of some of those middle stages in the kill chain, the actual malware, the exploits, the payloads, and the different methods of how they can be detected.

Conceptual model that illustrates the various impact of several of these indicators of compromise and measures the impact on advesaries when used for detection and response.

Emphasizes the idea that not all of these indicators are equal in their ability to disrupt an adversary's operation AKA cause them pain!

Not just an entire conceptual framework but can actively apply the concepts of the Pyramid of Pain in a more tangible way within our SOC.
(i.e. writing out detection rules)

Pyramid of Pain was developed by David Bianco as part of a discussion around detection strategies in his organization and the problem he had around trying to convey and describe and get across the idea that simply ingesting more and more threat intelligence is not the magical answer.

In an effort to argue how to best prioritize Cyber Intelligence data and get more value out of it, he developed this model to show how not all IOCs are created equal.

The pyramid consists of 6 different levels with each representing a different type of indicator or IOC, with the difficulty of the adversary changing their tactics increasing as we move up the pyramid.

We can correlate this to the Lockhart's Exchange Principle, which states that any contact leaves behind a trace, meaning that when two objects come into contact with one another, there is always an exchange of materials between them.

Within forensic science, it's the idea that the perpetrator of a crime will always bring something to the crime scene and leave taking something from it.

Both can be used for forensic evidence. This applies to computer crime or computer forensics as well.

What this means is that if a threat actor is doing something on our network, then they're leaving behind some kind of trace and they can't avoid that.

Our job is to find these traces and notice when those traces are being left within our network and response accordingly.
Or do somthing with them and respond accordingly or do something with them and disrupt whatever the attacker is doing in their kill chain.

and if we can find that indicator, then the attacker loses that method, or tool, or tactic or technique, and they then have to replace it. 
The difficulty of replacing that indicator or whatever created the indicator and the general pain it would cause the attacker would to to go through to replace it is what the Pyramid maps out.

### Different Levels

### Hash Values

Referring to static hash values so things like SHA-1 OR MD5 OR SHA-256 rather than any fuzzy hashes like SSDeep or other context-triggered hashes.

Unlike traditional hash functions like MD5 or SHA1 which generate a fixed size hash value regardless of the input size, we also have hashing algorithms and utilities like SSDeep that can produce a hash that's designed to be similar when the inputs are similar, even if there are small difference between the two files.

All of that is to say that we're focusing on the traditional cryptographic hashes like SHA-1 OR MD5 OR SHA-256.

When we collect a piece of malware say from a phishing email or extracted from a packet capture or an endpoint, we often have the means to obtain a file's hash, either manually or automatically and we can then go about creating detection rules to block that piece of malware if we were to come across it later on in the field.

However, the reason why hashes were at the bottom of the pyramid or classified as trivial is due to the very nature of how these hashes are built.
So we can have two identical files which will have the same file hash but if we were to change just a single bit, we would have wildly different hash values.

We can see how easy it is for an attacker to change the malware's hash value, and sometimes these hashes are so easily and susceptible to change, that they can even end up changing on their own, by accident. 

Say for some sort of transmission error that changed one of the bits or metadata was appended to the file, or recompiling the same malware at a later date could also change the hash.

So any detection rules around file hashes are not really causing that much pain to our adversaries.
Attackers have advanced far past the static hash signature detections and so not really a high value indicator.

### IP Addresses

Next and slightly more painful of an indicator but still relatively easy indicator.
We talked earler about why IP addresses are such fundamental indicators for malware, and somewhere we want to start when investigating endpoints, because you have to have some sort of network connection in order to carry out an attack or control and endpoint or exfiltrate data.

With connections, we are talking about the network so that will always be an IP address of some sort.
IP address indicators are just the address of the devices that carry out the attack
(i.e. attackers infrastructure, or a server they're using to stage the attack like command and control server, or IP of other affected endpoints as part of a larger botnet)

As analysts and responders, we might find IP addresses as Indicators of Compromise within packet captures or network protocol alerts or hardcocded into malware itself.

We have to remember the reason IP addresses are so low on the bottom of the pyramid is because they're pretty easy for an attacker to change.

If you block an attackers IP address from sending out emails, they can just move to a their email server to a different ip address or different email provider.

Especially with the abundance of cloud infrastructure, you can geta new IP address assigned to you pretty quickly and easily.

Not something an attacker is really tied to these days. Especially if they are using anonymous browsing service or something like TOR or an anonymous proxy.
An attacker's IP address might change around all the time, so not really an effective indicator for us.

Another reason why IP indicators aren't as high value is due to things like Content Delivery Networks, where we have legitimate services like Akamai, that distribute infrastructure across a large network of servers across the world.

If an attacker is doing something like this or rather, abusing it, to mask their true origin of traffic, it makes it hard to track and block.

Also things like FastFlux - technique used by attackers to hide phishing and malware delivery sites behind an ever-changing network of compromised hosts that are acting as proxies. Basic idea is to rapidly change the IP address associated with a domain name.

Obviously makes it much more challenging for us as defenders to block malicious activities based on IP addresses alone, since they're always switching around and hiding behind domain names.

### Domain Names

Slightly more pain than Hash Values and IP Addresses
A bit more trouble to go about registering a new domian name and dealing with registrars and paying for a domain but not much of a convern for a determined threat actors.

Very large number of DNS providers out there with very lax registration standards, some of which are free.
So again, in practice its not too hard to change domain names.

However,as we discussing during phishing section, we have technqiues to help with domain abuse, like blocking any new domains created within the last 30 days.

So if an attacker had to run out and register a brand new domain, well we'd proactively be blocking them once again.

However, to turn things back around on us, a determined attacker will likely have multiple domain names already staged with adequate domain ages and ready to go for an attack.

And again, we can typically find domain-related IOC's when we're looking at packet captures, so looking at any DNS requests, or at the live endpoint level,or through dynamic sandboxes. Again looking at any DNS queries that were made and what domains were contacted or sometimes we can find this within the malware itself.

If the attacker is using something like FastFlux or DynamicDNS then the domain has to be specified somewhere.
Using Lockhart's Exchange Principle, if its there then we can find it.

### Network/Host Artifacts

Speaking of the Exchange Principle, this brings us to different indications on what hosts or network level artifacts are left behind from the attacker.
Because as the attacker is doing things like exploiting their malware or dropping files on disks, or in the installation phase, carving out and installing persistence mechanisms and backdoors, there will inevitably be indicators in the form of artifacts or evidence on the host, like in the logs or autoruns locations or installed services and tasks. 

Also on the network level as well. 
Is there a registry key? We can think about the autostart locations that we talked about or the registry keys that get added when a service is installed.
Is there a specific file that gets dropped on disk, under a certain directory. 

Is there a certain way in which the command control channel is constructed.
Or is there a specific, specified user agent?
(i.e. we looked at user-agents in the wild like Southside or user-agents that contained slight misspellings.)

Maybe since we can't just rely on domains for detections, maybe the attacker is constantly changing their domain names but the URL patterns they use to recieve C2 traffic has a specific pattern we can recognize or write some regular expressions around to detect.

So we can do alot of the detections at this level using things like YARA and Sigma rules.

These Network and Host artifacts hold a bit more value and occupy a hgher place on the pyramid because they're more complex and difficult, or annoying for the attacker to change compared to the lower level indicators.

To get around these artifact level dections, the attacker will have to modify their tools, or modify code. 
This can be really small changes but the pain here is that the attacker doesn't know exactly what is being detected and will have to do a bunch of testing and recompiling.

Expanding on the hosts and network related indicators.

### Tools

Software and utilities the attackers use to execute their attacks.
(i.e. exploits, payloads)

Tools can range from custom bilt malware to pre-written exploits found online.

If we can start detecting entire tools and the way these tools work, it becomes genuinely challenging for adversaries to change or get around detections.

Can be a significant upfront cost to research, develop or purchase these tools.

Maybe they're using a specific piece of malware, while they can get around some of the lower level indicators, the actual payloads and the way the malware operates become burned or detected.

So the attacker really has no other option but to switch tooling.

Or it could be exploitation frameworks like Metasploit or Cobalt Strike and if we can detect these then the attacker will have to switch.

We usually get to this stage on the pyramid when all of our previous detection mechanisms have become so effective at identifying the artifacts of the tool itself in various ways. 
 
Because of this, the adversary is forced to abandoned the tool, and either find or develop a new tool to achieve the same purpose.

We can look at YARA or Sigma rules to develop these specific tool indicators or even things like fuzzy hashes, where we can perform more similarity analysis even if two binaries or files have minor differences.

Once we're detecting tools, we're making it challenging for the attacker to get around.

### TTPs

Really determined, highly sophisticated and financially backed, we may have to summit the pyramid.

Tactics, Techniques and Procedures

Behavior. The way in which the adversary is trained. Their preferences and the way those all come together in the form of activities on the network and systems.
No matter what tools they use or artifacts or IOCs like the domain names or IP addresses they use, it doesn't matter because now we're looking at the attacker through the lens of a very high level

On the tactics side, the high level objectives or goals the adversaries aim to achieve.

We can also think about Actions on Objectives as well. 
(i.e. an adversary's tactic might be to establish persistent access to a compromised system or exfiltrate sensitive data.


And the ways in which they go about exfiltrating data might be unique to their behavior.

#### Techniques

More detailed than tactics and describe how adversaries carry out their actual activities
(i..e technique for persistence might be to create a new user account or installing a services.)
(for exfiltration purposes, we could be looking at actual directories or filenames adversary uses - maybe they name their file Fubar.zip or they use a specific drive.)

All these small things that paint a picture of who this threat actor is, or essentially profiling.

Gold standard when it comes to looking at TTP's is MITRE ATT&CK Framework, specifically the Enterprise Matrix.

Maps out all sorts of TTP's that real threat actors use
(i.e.e reconnnaise, initial access, execution, persistence techniques, the ways in which attackers escalates privileges or moves laterally or sets up command and control.

If we start detecting and then attacking back against an adversary's training or geenral behavior of what action's they like to perform when they get initial access, or the ways in which they go about reconnaise or delivery, that's really tough for an attacker to get around.

It's behavior-based and things they do without even realizing it and like a habit, it's hard to change.

At this point they basically have two options, either painstakingly figure out what behavioral indicators we're detecting and then try to consciously change thieir behavior and training or proccedures, and while they're doing that- reinvest in tooling and everything else 

OR 

Find another target.

that's the point of the Pyramid of Pain, to chase them up the ladder or pyramid until it becomes too much of a pain and then they give up!

The extent you have to go to chase an adversary up the pyramid entirely depends on things like their motivation, resources, financial backing or sophistication

When we're talking about TTP's, we're thinking about Advanced Persistent Threats alot of the time and the data we have on their behavior.



















































































































































