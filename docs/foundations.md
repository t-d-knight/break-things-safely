# Get the Foundations

Cyber security sits on top of a bunch of other technologies.

You don't need to master all of them. You just need enough to understand what's happening underneath the security tooling.

If the acronyms on this page (or anywhere else on this site) stop making sense, the [Cyber & IT Glossary](glossary.md) is there to translate.

## The CIA triad

Before any of the technical foundations below, this is the concept almost every security course, cert and job ad assumes you already know — it's usually the literal first slide.

* **Confidentiality** — only the people who should see something can see it
* **Integrity** — data hasn't been tampered with or corrupted, and you'd know if it had
* **Availability** — the systems and data are actually there when someone legitimately needs them

Most security decisions are a trade-off between these three. Encrypting a hard drive protects confidentiality but can hurt availability if the recovery key gets lost. Locking an account after five failed logins protects against brute-forcing it, but a determined attacker can now weaponise that same lockout to deny the real user access. Neither answer is wrong — but being able to name which leg of the triad a decision is actually trading against is what "thinking like a security person" ([more on that here](think-like-a-pro.md)) starts with.

## Networking

Start by understanding:

* IP addresses
* DNS
* TCP and UDP
* Ports
* Routing
* Firewalls
* HTTP and HTTPS
* TLS
* Client/server communication
* What a packet actually contains

A security alert saying *"connection from 10.1.2.3 to TCP/443"* becomes considerably more useful when you know what those things mean.

## Linux

You don't need to become a Linux administrator.

Start with:

`ls` · `cd` · `cat` · `grep` · `find` · `curl` · `ssh` · `ps` · `ip` · `chmod`

Then start asking what each command actually does.

[TryHackMe](https://tryhackme.com) has beginner Linux material, and [OverTheWire](https://overthewire.org/wargames/) has excellent games for learning Linux and security concepts by solving problems.

## Windows and Active Directory

Most Australian workplaces run on Windows, and a lot of them run on **Active Directory** — the system that manages user accounts, permissions and machines across a whole organisation from one place. This is a genuine gap in a lot of beginner material, which tends to assume Linux is the only operating system worth learning.

Start with:

* Navigating Windows without a mouse — File Explorer, Control Panel, Task Manager, Event Viewer
* [PowerShell](https://learn.microsoft.com/en-us/powershell/) — Windows' equivalent of the Linux command line, and increasingly how both admins and attackers actually interact with Windows
* What a **domain**, a **domain controller**, a **user account** and a **group** actually are
* **Group Policy** — how an organisation pushes settings to every machine at once

[TryHackMe's Windows Fundamentals](https://tryhackme.com/room/windowsfundamentals1xbx) series (parts 1 to 3) is free and covers the basics from nothing. Once that's comfortable, [Active Directory Basics](https://tryhackme.com/room/winadbasics) — also free — introduces the concepts that show up constantly in SOC, IT support and pentesting job ads alike.

If you want to build your own, [Build Your Own Lab](build-a-lab.md) covers setting up a domain controller and a joined client using Microsoft's own free evaluation software — genuinely the best way to see how it all fits together.

## Programming

You don't need to become a software developer.

Learning some Python is enough to start automating repetitive tasks, processing data and building little tools.

[Exercism](https://exercism.org) provides free programming exercises in dozens of languages.

A good rule:

!!! tip "Rule of three"
    If you find yourself doing something more than three times, consider writing a script to do it for you.
