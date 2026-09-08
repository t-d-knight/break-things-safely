# Learn to Think Like a Security Person

Cyber security isn't just memorising tools.

It's learning to ask better questions.

## "How bad is this?"

CVSS gives vulnerabilities a severity score.

But:

!!! info "Remember"
    CVSS is a severity score, not a priority score.

A critical vulnerability on an isolated machine may be less urgent than a high-severity vulnerability on an internet-facing authentication server.

Consider:

* Can an attacker reach it?
* Does it require authentication?
* Does it require user interaction?
* Is exploitation known to be happening?
* What does the vulnerable system have access to?
* What happens if it is compromised?
* Are there compensating controls?

That's the beginning of risk-based security thinking.

## MITRE ATT&CK

[MITRE ATT&CK](https://attack.mitre.org)

ATT&CK provides a common language for describing attacker tactics and techniques.

You don't need to memorise it.

Start using it to ask:

!!! info "The ATT&CK question"
    What was the attacker trying to achieve, and what technique did they use to do it?

That's how a lot of professional SOC, detection and threat-intelligence work starts to make sense.

## The Essential Eight (and what's replacing it)

[The Essential Eight](https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/essential-eight) is the Australian Signals Directorate's set of eight baseline mitigation strategies — things like patching, application control and restricting admin privileges — ranked against a maturity model. If you've been anywhere near Australian government or enterprise security, you've seen it.

Worth knowing going in: in June 2026 the ACSC announced the Essential Eight is being retired over roughly the next two years, replaced by a broader set of guidance called the **Essentials series** — organised by technology domain (enterprise IT first, cloud and operational technology to follow) instead of one fixed eight-control checklist. Nothing about current obligations has changed yet, and existing Essential Eight work is expected to map across rather than get thrown out.

Treat it as a snapshot, not gospel — a specific moment in Australian cyber security policy, already a little dated in places, but still the fastest way to understand how a huge number of Australian organisations think about baseline security today. Worth learning the current framework and watching the Essentials series roll out around it, not skipping straight past it.

### Try the Navigator

[ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/) turns that theory into something visual. Pick a few threat actor groups that target your industry and layer their known techniques on top of each other — the overlap is the useful bit. Techniques shared by several groups are usually the ones worth defending against first.

That's a real introduction to threat modelling and control prioritisation, not just a theory exercise. [HackerSploit's Navigator walkthrough](https://www.youtube.com/watch?v=hN_r3JW6xsY) shows the idea in a few minutes.
