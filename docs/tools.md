# Security Tools We Actually Use

These tools are useful for investigating files, domains, IP addresses and security events.

!!! danger "The golden rule"
    If you don't own it and you don't have permission to test it, don't test it.

Your own devices, your own accounts, deliberately vulnerable labs and CTF platforms are fair game.

Pointing scanners at somebody else's systems because *"I was only learning"* isn't a defence.

**Also think before you upload anything.**

These are security research platforms, not private dumping grounds.

Don't upload:

* Personal documents
* School assignments containing personal information
* Private photographs
* Passwords or authentication tokens
* Confidential work material
* Someone else's information

If the material belongs to your school, employer or someone else, ask first.

## What if you find something you shouldn't have

Sometimes you're not looking, and you stumble onto a real vulnerability on a real, live system that isn't yours. That's a different situation to deliberately testing something without permission — but it still needs handling carefully.

Don't dig further than you need to confirm it's real. Don't access, download or change any data beyond that. Don't tell anyone publicly before the organisation knows.

This site doesn't have day-to-day experience running disclosure processes, so rather than improvise, use the reputable references built specifically for this:

* [disclose.io](https://disclose.io) — plain-language guidance and templates for reporting a vulnerability responsibly, including how to find the right contact for an organisation that hasn't published one
* [The CERT Guide to Coordinated Vulnerability Disclosure](https://certcc.github.io/CERT-Guide-to-CVD/) — the long-form reference from CERT/CC (Carnegie Mellon's CERT Coordination Center) on how responsible disclosure is meant to work and why

If you're a minor or otherwise unsure, loop in a parent, teacher or someone else you trust before reaching out to the organisation — see [If Something Actually Goes Wrong](if-something-goes-wrong.md) for the general "get help early" principle, which applies here too.

| Tool                                                         | What it does                                                |
| -------------------------------------------------------------- | -------------------------------------------------------------- |
| [Wireshark](https://www.wireshark.org)                       | Capture and inspect network traffic packet by packet — see [Build Your Own Lab](build-a-lab.md) for how to actually get traffic to look at |
| [Nmap](https://nmap.org)                                     | Scan a network to find live hosts, open ports and running services — the golden rule above applies to this one more than any other tool on this page |
| [VirusTotal](https://virustotal.com)                         | Analyse files, URLs and hashes using many security engines  |
| [Cisco Talos](https://talosintelligence.com)                 | Threat intelligence and reputation information              |
| [AlienVault OTX](https://otx.alienvault.com)                 | Community-driven threat intelligence                        |
| [ANY.RUN](https://any.run)                                   | Interactive malware sandbox                                 |
| [URLScan.io](https://urlscan.io)                             | Inspect what happens when a URL is loaded                   |
| [Shodan](https://shodan.io)                                  | Search engine for internet-exposed devices                  |
| [Spur](https://spur.us)                                      | IP address and infrastructure context                       |
| [crt.sh](https://crt.sh)                                     | Search certificate transparency data                        |
| [WhereGoes](https://wheregoes.com)                           | Trace URL redirects                                         |
| [WHOIS](https://whois.domaintools.com)                       | Domain registration information                             |
| [Have I Been Pwned](https://haveibeenpwned.com)              | Check whether an email address appears in known breaches    |
| [CyberChef](https://gchq.github.io/CyberChef)                | Decode, transform and analyse data                          |
| [abuse.ch](https://abuse.ch)                                 | Malware and botnet threat intelligence                      |
| [MACVendors](https://macvendors.com)                         | Identify a device manufacturer from a MAC address           |
| [CVSS Calculator](https://www.first.org/cvss/calculator/3.1) | Understand how vulnerability severity scores are calculated |

