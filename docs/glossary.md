# Cyber & IT Glossary

Cyber security runs on acronyms. People who've been in the industry a while forget that "just spin up a VM, check the IOCs against the SIEM and see if it's related C2" is a completely different language to someone starting out.

This isn't every term in the industry — it's the ones you'll actually run into reading the rest of this site, a job ad, or a news article about a breach.

!!! tip "Don't try to memorise this"
    Nobody learns a glossary front to back. Bookmark this page and come back when something in a course, tool or article doesn't make sense.

## Networking basics

| Term | Meaning |
| --- | --- |
| IP address | The numeric address a device uses to send and receive data on a network |
| DNS | Domain Name System — translates a website name like `example.com` into an IP address |
| TCP / UDP | The two main ways data gets packaged and sent across a network — TCP double-checks delivery, UDP just sends it |
| Port | A numbered "door" on a device that a specific type of traffic goes through, e.g. 443 for HTTPS |
| HTTP / HTTPS | The protocol web traffic uses to move between a browser and a website — the "S" means it's encrypted |
| TLS / SSL | The encryption that makes the "S" in HTTPS possible — TLS is the modern version, SSL is the old, retired one people still say out of habit |
| VPN | Virtual Private Network — routes your traffic through an encrypted tunnel, usually to hide it from your network or change your apparent location |
| Firewall | A system that allows or blocks network traffic based on a set of rules |
| MAC address | A hardware address unique to a specific network device, separate from its IP address |

## Accounts, access and identity

| Term | Meaning |
| --- | --- |
| MFA | Multi-Factor Authentication — proving who you are with more than just a password, e.g. a code from an app |
| 2FA | Two-Factor Authentication — MFA with exactly two factors |
| SSO | Single Sign-On — one login that grants access to multiple systems |
| IAM | Identity and Access Management — the systems and processes controlling who can access what |
| RBAC | Role-Based Access Control — access is granted based on a person's role, not individually per person |
| Least privilege | The principle that someone should only have the access they actually need to do their job, nothing more |
| PAM | Privileged Access Management — extra controls around high-value accounts like admins |
| Zero Trust | A security model built on "never trust, always verify" — nobody and nothing gets automatic access just for being inside the network perimeter, every request gets checked on its own merits |

## Threats and attacks

| Term | Meaning |
| --- | --- |
| Malware | Any software designed to cause harm — an umbrella term covering viruses, ransomware, spyware and more |
| Ransomware | Malware that encrypts a victim's files and demands payment to unlock them |
| Phishing | A fake message designed to trick someone into handing over credentials or installing malware |
| Smishing / Vishing | Phishing over SMS text (smishing) or a phone call (vishing) instead of email |
| Social engineering | Manipulating a person, rather than a system, into doing something insecure |
| RAT | Remote Access Trojan — malware that gives an attacker remote control of an infected device |
| C2 | Command and Control — the infrastructure an attacker uses to control compromised devices remotely |
| DDoS | Distributed Denial of Service — flooding a system with traffic from many sources to knock it offline |
| Zero-day | A vulnerability that's being exploited before the vendor has released a fix for it |
| APT | Advanced Persistent Threat — a well-resourced attacker (often state-linked) running a long-term, targeted campaign rather than a smash-and-grab |
| IOC | Indicator of Compromise — a piece of evidence (a file hash, an IP, a domain) that suggests a system has been breached |
| TTP | Tactics, Techniques and Procedures — the patterns of behaviour a particular attacker or attack tends to follow |

## Defending and responding

| Term | Meaning |
| --- | --- |
| SOC | Security Operations Centre — the team that monitors for and responds to security events |
| SIEM | Security Information and Event Management — a system that collects and correlates logs from across an organisation to spot suspicious activity |
| IDS / IPS | Intrusion Detection/Prevention System — watches network traffic for known-bad patterns; IDS alerts on it, IPS actively blocks it |
| EDR / XDR | Endpoint (or Extended) Detection and Response — software that monitors individual devices for malicious activity and can respond automatically |
| SOAR | Security Orchestration, Automation and Response — tooling that automates the repetitive parts of responding to an alert, so a human only steps in for the parts that actually need judgement |
| IR | Incident Response — the process of investigating and containing a security incident once it's detected |
| DLP | Data Loss Prevention — tools and rules that stop sensitive data leaving an organisation |
| Patch | An update that fixes a known bug or vulnerability |
| Pen test | Penetration test — an authorised, simulated attack against a system to find weaknesses before a real attacker does |
| Red team / Blue team | Red team attacks (simulating a real adversary), blue team defends — some roles do both and are called purple team |

## Vulnerabilities and scoring

| Term | Meaning |
| --- | --- |
| CVE | Common Vulnerabilities and Exposures — a public reference number assigned to a specific known vulnerability |
| CVSS | Common Vulnerability Scoring System — a 0–10 score representing how severe a vulnerability is |
| CWE | Common Weakness Enumeration — a category of vulnerability type (e.g. "SQL injection"), as opposed to one specific instance of it |

## Frameworks, standards and roles

| Term | Meaning |
| --- | --- |
| MITRE ATT&CK | A public knowledge base cataloguing real-world attacker tactics and techniques, widely used as a reference framework |
| Essential Eight (E8) | ASD's eight baseline mitigation strategies for Australian organisations — being retired and replaced by the broader [Essentials series](think-like-a-pro.md#the-essential-eight-and-whats-replacing-it) from 2026, but still the reference point most Australian orgs use today |
| NIST | National Institute of Standards and Technology — a US body whose cyber security frameworks are widely used as best-practice references worldwide |
| ISO 27001 | An international standard for managing information security within an organisation |
| GDPR | General Data Protection Regulation — the EU's data privacy law, widely used as a reference point even outside the EU |
| PII | Personally Identifiable Information — data that can identify a specific individual |
| CISO | Chief Information Security Officer — the executive responsible for an organisation's security |

## General IT terms you'll see used casually

| Term | Meaning |
| --- | --- |
| OS | Operating System — Windows, macOS, Linux and so on |
| VM | Virtual Machine — a simulated computer running inside another computer, used constantly for safe testing and labs |
| CLI / GUI | Command Line Interface (typed commands) vs Graphical User Interface (windows and clicking) |
| API | Application Programming Interface — a defined way for one piece of software to talk to another |
| SaaS | Software as a Service — software hosted and run by someone else, accessed over the internet rather than installed |
| Cloud | Computing resources (servers, storage) rented from someone else's data centre instead of run on your own hardware |
| Repo | Repository — a folder of code (and its history) tracked with a version control tool like Git |
| Hash | A short, fixed-length fingerprint generated from a file or piece of data, used to verify it hasn't changed |

---

If a term you've hit isn't here, that's worth flagging — [open an issue or a pull request](https://github.com/t-d-knight/break-things-safely) and it can be added.
