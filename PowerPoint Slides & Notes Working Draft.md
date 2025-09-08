## Slide 1 - Opening & Introduction

Good morning, everyone!

Before we jump into the nitty-gritty of cybersecurity, let's take a moment to get to know each other.

## Slide 2 - Intro Injection Slide

I'd love to know: I***s this anyone's first BSides conference?***

-Raise your hand if that's you!

_(Pause for audience response)_

Awesome! Welcome aboard! My first conference ever was this past April at BSidesSLC, and it was a total blast.

These events are all about networking, learning and contributing to the community and industry. I'm pumped to be here with you today, if you'd like, feel free to add me on LinkedIn!

## Slide 3 - My Non‑Linear Journey

***My road to presenting about Cybersecurity today?*** 
	Well, Let's just say it's been a wild ride. I've scrubbed toilets, driven trains, and if you're wondering, yes, I was at the engineering console of the FrontRunner. Hopefully I didn't leave you behind on the last run of the night. 

I've repaired phones, managed teams, worked help desks, and currently work for an inventory management software company providing cloud support.

Every single position has taught me something new whether it be grit, problem-solving, or how to pivot when things get messy. Believe, me, it will get messy. Over Labor Day weekend, I was on call having just Discovered, Contained, and Eradicated the Zeppelin Ransomware created by Vice Society the Friday before a long weekend. 

Fortunately, we caught the piece of malware before it propagated, which allowed an ideal weekend.

-Together, all of these elements come together to support my core principles and keep me going every day.

## Slide 4 - Big Wins & Real Challenges

If you asked me what a normal day looked like, I couldn't give you a real answer. I've had the opportunity to work with some heavy hitters such as Hershey's Chocolate, Pepsi, McDonald's, the U.S. Department of Homeland Security, the U.S. Army, the U.S. Air Force, and even NASA.

I'm the Ambassador for the Northern Utah area for Simply Cyber, shutout to #TeamSC!

If you haven't checked it out, Simply Cyber is a SANS-awarded podcast that runs every weekday.

- It's been a goldmine for helping me to stay sharp in the industry, earn free CPEs, and make some incredible friends along the way. If you aren't already there, join us in Discord. If you are, top by the #locals-info room and get your role to join our areas room. 
-You can check it out by visiting simplycyber.io/discord
## Slide 5 - Where Cybersecurity Meets Humanity

Why share all this?

Because throughout all the different industries I've worked in, I've learned that tech debt has far reaching arms.
	I've witnessed first hand that Cybersecurity isn't just scripts, logs, and punching through firewalls.
		It's about the people behind each project, each team, each interaction, and the experiences that shape us.

Today, I'm here to talk about turning challenges into strengths, and I can't wait to dive in with you, so let's get started.
	But first I must apologize that while I don't have the time to get through all of what I wanted to share, I will make it available on my GitHub. If you're interested, come see me after.


## Slide 6 - Technical Debt: A Hidden Threat

**Cybersecurity's Critical Role** is that it protects business operations by safeguarding data, ensuring continuity, and maintaining customer trust.

A 2021 IBM report estimated the average cost of a data breach at $4.25 million, highlighting the financial impact for businesses. [ftc](https://www.ftc.gov/business-guidance/blog/2019/07/575-million-equifax-settlement-illustrates-security-basics-your-business)
	Outdated systems, unpatched software, and misconfigurations create vulnerabilities that adversaries exploit, increasing the risk of breaches such as the 2017 Equifax incident. [barradvisory](https://www.barradvisory.com/wp-content/uploads/2022/05/The-Impact-of-Technical-Debt-on-Cybersecurity.pdf)

Technical debt amounts to 20-40% of an organization's technology estate value, positioning it as a business risk multiplier. [barradvisory](https://www.barradvisory.com/wp-content/uploads/2022/05/The-Impact-of-Technical-Debt-on-Cybersecurity.pdf)

**Bridging Perspectives**: Effective communication translates technical risks into business terms (e.g., financial losses, reputational damage), securing executive buy-in and resources.

## Slide 7 - Bridging Perspectives

(Ask Audience rhetorically) "What would a week-long system outage cost your business?" 

"Do you know how much a day-long outage would cost your organization?"

_pause_

"A week?"

_pause_

"A month?"

"Imagine, if you will with me for a moment, technical debt like rust on a bridge. At first it seems cosmetic, but when left unchecked it weakens the entire structure. 'Good enough' might hold for now, but it inevitably multiplies risk until the bridge, or your infrastructure, fails."
	This is just a preview, now let's dive deeper into understanding Risk, so we can learn how to translate  technical risk ratings into business impact metrics. The key you'll see is moving from “what can break” and "how bad is it broken" to “what it means when it breaks.”
## Slide 8 - The Lockheed Martin Cyber Kill Chain Framework

The Lockheed Martin Cyber Kill Chain is a framework that outlines the stages of a cyber-attack, from initial reconnaissance to achieving the attacker’s objective.
	It helps organizations understand and detect threats at each phase, enabling better defense and response strategies.
		By breaking down the attack life-cycle, it highlights opportunities to stop intrusions before they succeed.

The standard seven stages are:

1. **Reconnaissance** - Attackers gather information about the target, such as vulnerabilities, technologies used, and organizational structure, using public sources, social engineering, or network scanning.
  
2. **Weaponization** - Cyber adversaries create or tailor malware, viruses, or exploit code specifically for the discovered vulnerabilities, bundling payloads and exploits into a deliverable format (often via automated tools).
  
3. **Delivery** - The payload is transmitted to the target, most commonly through email attachments, malicious links, compromised websites, or USB devices.

4. **Exploitation** - The delivered malicious code is executed on the victim's system, taking advantage of vulnerabilities to gain initial access.    

5. **Installation** - Attackers install malware or backdoors, establishing a persistent presence on the target system for future access.

6. **Command and Control (C2)** - The attacker establishes communication channels to remotely control the infected system, exfiltrate data, or issue further instructions to the malware.    
 
7. **Actions on Objectives** - The final step involves carrying out the attacker's goals, such as data theft, destruction, ransomware deployment, or espionage.


**Key Context**:

- The Cyber Kill Chain was adapted from the military concept of the kill chain, emphasizing that if defenders disrupt any stage, the attack can be contained or stopped. [lockheedmartin](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)

- The Cyber Kill Chain is particularly effective for modeling Advanced Persistent Threats (APTs) and enables organizations to strengthen defenses at each stage, from perimeter monitoring to internal detection and incident response. [lockheedmartin](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)


## Slide 9 - Case Study: Equifax Breach (2017)

During the **2017 Equifax Breach** an unpatched Apache Struts vulnerability ultimately led to a data breach affecting 147 million people, costing at least $1.4 billion in damages. [ftc+1](https://www.ftc.gov/news-events/news/press-releases/2019/07/equifax-pay-575-million-part-settlement-ftc-cfpb-states-related-2017-data-breach)

**Timeline**: Disclosed March 7, 2017; DHS notified Equifax March 8; internal patching failed; exploited May 13-July 29, 2017. [archive.epic](https://archive.epic.org/privacy/data-breach/equifax/)

This use case has some key technical debt factors, such as incomplete IT asset inventory, failed patch management, expired security certificates due to disabled monitoring for 19 months, and legacy system complexity dating back to the 1970s. [sevenpillarsinstitute+1](https://sevenpillarsinstitute.org/case-study-equifax-data-breach/)

### How Technical Debt Enabled the Equifax Breach Through the Kill Chain:

| **Kill Chain Stage**      | **Attack Actions**                                                                       | **Technical Debt Enablers**                                                                                                                                                                                       | **Prevention Strategies**                                 |
| ------------------------- | ---------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| **Reconnaissance**        | Attackers identified publicly accessible Equifax systems and Apache Struts vulnerability | Lack of comprehensive IT asset inventory made systems discoverable [sevenpillarsinstitute](https://sevenpillarsinstitute.org/case-study-equifax-data-breach/)                                                     | Complete asset inventory, reduce external footprint       |
| **Weaponization**         | Crafted malicious HTTP payload exploiting CVE-2017-5638                                  | Known vulnerability remained unaddressed for months [blackduck](https://www.blackduck.com/blog/cve-2017-5638-apache-struts-vulnerability-explained.html)                                                          | Automated vulnerability management, threat intelligence   |
| **Delivery**              | Sent malicious HTTP requests to ACIS dispute portal                                      | Web application lacked proper input validation [blackduck](https://www.blackduck.com/blog/cve-2017-5638-apache-struts-vulnerability-explained.html)                                                               | Web Application Firewall (WAF), input sanitization        |
| **Exploitation**          | Executed arbitrary commands via Apache Struts vulnerability                              | Critical patch not applied within 48-hour policy window [ftc](https://www.ftc.gov/business-guidance/blog/2019/07/575-million-equifax-settlement-illustrates-security-basics-your-business)                        | Enforced patch management, automated compliance checking  |
| **Installation**          | Used default "admin" credentials to establish persistent access                          | Default credentials unchanged, no multi-factor authentication [ftc](https://www.ftc.gov/news-events/news/press-releases/2019/07/equifax-pay-575-million-part-settlement-ftc-cfpb-states-related-2017-data-breach) | Strong password policies, mandatory MFA implementation    |
| **Command & Control**     | Established covert channels for 76 days undetected                                       | Expired SSL certificates disabled network monitoring for 19 months [itassetmanagement](https://itassetmanagement.net/2019/02/15/equifax-and-cybersecurity-a-deep-dive/)                                           | Active certificate management, continuous monitoring      |
| **Actions on Objectives** | Exfiltrated 147 million consumer records                                                 | No network segmentation, lack of Data Loss Prevention (DLP) systems [mit](https://web.mit.edu/smadnick/www/wp/2020-19.pdf)                                                                                        | Network segmentation, DLP deployment, data classification |

## Slide 10 - Case Study: SolarWinds Attack (2020)

During the **2020 SolarWinds Attack**, technical debt in supply chain security exposed over 18,000 organizations via a compromised software update. [attack.mitre+1](https://attack.mitre.org/campaigns/C0024/)

It went undetected for 15 months (September 2019 - December 2020), highlighting the risk of inheriting technical debt from third-party relationships. [techtarget](https://www.techtarget.com/whatis/feature/SolarWinds-hack-explained-Everything-you-need-to-know)

### How Technical Debt Enabled the SolarWinds Attack Through the Kill Chain:

| **Kill Chain Stage**      | **Attack Actions**                                               | **Technical Debt Enablers**                                                                                                                                                                   | **Prevention Strategies**                                      |
| ------------------------- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| **Reconnaissance**        | APT29 studied SolarWinds' code structure and build processes     | Insufficient visibility into software supply chain dependencies [aquasec](https://www.aquasec.com/cloud-native-academy/supply-chain-security/solarwinds-attack/)                              | Software Bill of Materials (SBOM), third-party risk assessment |
| **Weaponization**         | Developed SUNSPOT malware to inject SUNBURST into build pipeline | Insecure software development lifecycle practices [rapid7](https://www.rapid7.com/blog/post/2021/01/12/update-on-solarwinds-supply-chain-attack-sunspot-and-new-malware-family-associations/) | Secure Software Development Framework (SSDF), code signing     |
| **Delivery**              | Distributed trojanized Orion updates to 18,000+ customers        | Compromised build environment with privileged access [crowdstrike](https://www.crowdstrike.com/en-us/blog/sunspot-malware-technical-analysis/)                                                | Secure CI/CD pipeline, build environment isolation             |
| **Exploitation**          | SUNBURST backdoor activated after 2-week dormancy period         | Lack of behavioral monitoring and anomaly detection [thesslstore](https://www.thesslstore.com/blog/all-you-need-to-know-about-the-solarwinds-hack/)                                           | Advanced threat detection, behavioral analytics                |
| **Installation**          | Deployed TEARDROP and RAINDROP for persistent access             | Weak access controls and credential management [cyberark](https://www.cyberark.com/resources/blog/the-anatomy-of-the-solarwinds-attack-chain)                                                 | Zero Trust architecture, privileged access management          |
| **Command & Control**     | Established covert channels mimicking legitimate Orion traffic   | Insufficient network segmentation and monitoring [cisecurity](https://www.cisecurity.org/solarwinds)                                                                                          | Network segmentation, advanced SIEM capabilities               |
| **Actions on Objectives** | Selective targeting of high-value organizations for espionage    | Limited incident response capabilities and threat hunting [attack.mitre](https://attack.mitre.org/campaigns/C0024/)                                                                           | Proactive threat hunting, enhanced incident response           |

## Slide 11 - Kill Chain × Technical Debt

As shown in the Equifax, and SolarWinds breaches, Technical debt can create vulnerabilities at every stage of the attack chain, making it critical to identify and address these issues proactively. Reducing technical debt strengthens defenses across the attack chain, minimizing the likelihood of a successful attack. [bitsight+1](https://www.bitsight.com/blog/tackling-technical-debt-cybersecurity-veterans-guide)

## Slide 12 - Four Translation Techniques

When we talk about translating technical risk into business terms, there are a few techniques that really help the message land.

**First**, we can **quantify risks**. Models like FAIR let us express them in dollars and cents. Instead of just saying, “This system has a critical vulnerability,” we can say, “There’s a 30% chance this weakness could cost us $2 million if exploited.” Suddenly, leadership has something concrete to weigh.

**Second**, we need to **highlight operational impacts**. Technical debt doesn’t just live in code—it shows up when systems go down, when employees lose hours of productivity, or when ransomware keeps us offline for days. These are costs the business immediately feels.

**Third**, don’t underestimate **reputational damage**. A single breach can undo years of trust-building with customers and partners. Think about Equifax, the technology failed, yes, but the real story was how quickly confidence in the brand collapsed.

**Another** powerful tool is **analogy**. Sometimes the best way to connect is by comparing risk to something familiar: “A vulnerability is like leaving the lock broken on your storefront—it may look fine from the outside, but it’s an open invitation.”

Finally, we have to **provide clear metrics**. Pair qualitative measures, like CVSS scores, with quantitative ones, like projected financial losses. That’s how we make risk tangible, relatable, and actionable.

## Slide 13 - C‑Suite Communication Map

Cybersecurity professionals often use technical jargon (e.g., CVEs, TTPs) that consistently fails to resonate with executives and other senior leadership members who are focused on revenue, customer trust, and compliance.

Effective communication helps to align cybersecurity with business priorities, securing stakeholder buy-in. Remember, you don't need to dumb anything down, you're simply translating it from a technical explanation to one of business impact.

## Slide 14 - Why Translation Fails & How to Fix It

Instead of saying, "We need to patch CVE‑2025‑22224 in our software," say, "An unpatched vulnerability could lead to a $2 million data breach, disrupt operations for three days, and damage our reputation with customers."

**Key Takeaway**: Translating technical risks into financial, operational, and reputational impacts ensures executives understand and prioritize cybersecurity in accordance with business goals. Translating security risk and activities into a business dialect will increase stakeholder buy-in, participation, and even budgets.


## Slide 15 - Prioritization Strategies

When it comes to tackling technical debt, the real challenge isn’t just finding it, it’s knowing how to prioritize it.

The first strategy is **regular audits**. Think of it like a health check-up. You have to ask: what’s outdated, what’s unpatched, and where are the cracks forming?
	Without those touchpoints, debt piles up silently.

From there, we shift to **risk-based prioritization**. Not every issue deserves the same level of urgency. Frameworks like CVSS or CISA’s KEV catalog can help us focus attention on the debts that have higher likelihood of turning into real-world breaches.

But prevention is just as important as response. That’s where **DevSecOps** comes in. By embedding security throughout the software development lifecycle, we can build securely from the beginning, rather than trying to bolt on security after initial development.

Of course, this can't can’t be done strictly manually. You'll need to **automate** wherever possible, scanning for vulnerabilities, patching, and compliance checks. Automation doesn’t just save time; it keeps organizations from falling behind where attackers can move much faster.

Finally, we need to **assess asset criticality**. Some systems are simply more important than others. If an asset contains sensitive data or supports core operations, it should move to the top of the list.

When you combine all of these, you start to turn technical debt from an overwhelming liability into something reasonably manageable. It’s not about eliminating everything all at once, it’s about tackling the right debts at the right time, so you can protect the business and keep moving forward.

## Slide 16 - Four‑Quadrant Debt Model

Think of the **Four-Quadrant Technical Debt Model** like maintaining your house. Sometimes you **deliberately** put off fixing something, like leaving the old water heater in place for one more season, if you’re planning for it, that can be _prudent_. 

However, if you ignore a leaking roof because it feels inconvenient, that’s _reckless_. Other times, debt happens **inadvertently**, like discovering old wiring hidden in the walls. If you spot it early and plan the repair, that’s prudent; if you don’t even know it’s there until the breaker trips, that’s reckless.

The model helps us see not just the cost of maintenance, but whether the debt we carry is intentional and manageable, or risky and dangerous.
## Slide 17 - Implementation Roadmap

Sticking with home repair, think of the Implementation Roadmap like caring for a house.

- **Phase 1** is inspecting everything and making a list.
- **Phase 2** is fixing the easy leaks and broken locks.
- **Phase 3** is tackling big renovations like replacing the roof.
- **Phase 4** is ongoing upkeep so the house stays strong over time.

## Slide 18 - Building the Business Case

- To build a strong business case, start by **calculating the cost of inaction**, showing what breaches could cost in real dollars. 
- Then **demonstrate ROI**, proving how remediation investments sharply reduce those risks, often by orders of magnitude. 
- Tie your efforts directly to **business goals** like compliance, resilience, and customer trust, and **engage stakeholders** with data-driven metrics and real-world examples.
- Finally, shift from reactive fixes to proactive management by embedding technical debt into enterprise risk frameworks and fostering a culture of continuous improvement.
- The takeaway: remediation isn’t just security work, it’s a strategic business initiative.


## Slide 19 - Summary & Call to Action

**Closing Thought**: By speaking security with a business accent, ***you*** will turn technical challenges into opportunities for organizational resilience, fostering collaboration and driving meaningful change.

Closing Statement

Technical debt ***is*** inevitable.

(Pause)

but so is progress. 

(SLOW DOWN)

If we face it head-on, we don’t just reduce risk. We build ***resilience***, ***trust***, and a ***stronger future***. Thank you for your time today.
