# Introduction
The Morris worm was introduced in 1988 by Robert Tappan Morris and is often considered one of the first public cyber attacks, resulting in the first felony conviction under the US 1986 Computer Fraud and Abuse act. [1]

It was launched at 8:30pm 02.11.1988 from the Massachusetts Institute of Technology, Morris himself being a student at Cornell university but releasing from MIT in the hopes of hiding his identity. Although it poses no threat today, as a modern computer is immune to the vulnerabilities it exploited, it did go on to inspire generations of hackers who still use worms in attacks today, as well as generating some first suspicions about information used and stored online. [2]

# Who Was Attacked
As the attack came a year before the invention of the world wide web, the current national electronic network was made up of a number of systems at prestigious colleges and research centres. The worm spread through this network, targeting computers running a specific version of UNIX OS but spread widely as it featured multiple vectors of attack as well as being designed to stay hidden.[3] Within 24 hours of its release an estimated 2000-6000 of the then (also estimated) 60000 computers connected to the internet were affected. 

# Effects of the attack

When creating the worm Morris' coding instructed it to replicate regardless of whether the machine was infected or not, and the resulting level of replication turned the worm into a viral DoS attack [1]. The worm slowed machines to a crawl, with emails and vital military/university functions taking days to complete. In order to combat it, some organisations wiped their systems or disconnected from the network for up to a week. Ironically, Morris did attempt to apologise publicly and give guidance on removing the worm through a friend after seeing its effects but due to the damage caused to the network few recieved this message in time [3]. 

It is estimated that the total impact of the attack cost between 100,000 and 10,000,000, but many say the real cost comes from the psychological impact it had on the perception of security and reliability on the internet [1]. The attack also prompted DARPA to fund the CERT/CC at Carnegie Melon University in order to create a central point for experts to respond to future network emergencies.

Morris himself faced 3 years jail time and then probation, 400 hours of community service, a fine of 10,050USD, as well as years in court.

# Vulnerability exploited

The Morris worm was able to spread so effectively due to its exploitation of several vulnerabilities, including a hole in the debug mode of the UNIX sendmail program, a buffer overflow in the finger network service, and the transition trust enabled by people setting up network logins with no password requirements via remote execution. It also exploited weak passwords. 

The worm used a 'grappling hook' to download its main body parts and the hook would then run on other systems, making them peripheral victims.

Another method used by morris was almost accidental. The worm was initially programmed to check whether the computer it was spreading to was infected, but he realised that some sysadmins might counter this by sending it a false positive. To counteract this he programmed the worm to copy itself 14% of the time regardless of the machines infected status. This resulted in each machine potentially being infected multiple times, with each additional infection causing the machines to slow down to unusability, and eventually crashing the computer (similar to the effect created by a fork bomb) [1]

# STRIDE Model
**Spoofing**: Morris used weak passwords or lack thereof to gain access to systems. \
**Tampering**: The worm self replicated across syste,s. \
**Repudiation**: This aspect is less relevant. \
**Information Disclosure**: Less relevant. \
**Denial of Service (DoS)**: The worm acted as a DoS attack, shutting down systems/causing them to be wiped/disconnected. \
**Elevation of Privilege**: The worm overrode the sysadmins ability to stop it via random self copying.
# References
- [1]https://en.wikipedia.org/wiki/Morris_worm
- [2]  https://www.okta.com/uk/identity-101/morris-worm/#:~:text=A%20hacker%20launched%20the%20Morris,worm%20inspired%20generations%20of%20hackers.
- [3] https://www.fbi.gov/news/stories/morris-worm-30-years-since-first-major-attack-on-internet-110218

## Credit
- Josephine Baldry