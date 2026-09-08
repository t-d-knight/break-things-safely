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
