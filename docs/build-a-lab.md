# Build Your Own Lab

You don't need an expensive computer.

A spare PC, decent laptop or even a reasonably powerful desktop can become a cyber lab.

| Option                                                                                                                                                    | What it gives you              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- |
| [Proxmox](https://www.proxmox.com)                                                                                                                        | Free virtualisation platform   |
| [Windows Sandbox](https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/windows-sandbox-overview) | Disposable Windows environment |
| [VirtualBox](https://www.virtualbox.org)                                                                                                                  | Free desktop virtualisation    |
| [VMware Workstation Pro](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)                                                       | Free desktop virtualisation — now free for personal use, worth knowing since VMware's everywhere in the industry |

For hosted, ready-to-go labs rather than building your own, see the platforms in [Get Hands-On](hands-on.md) — TryHackMe and OverTheWire are the easiest starting points.

A lab lets you break things without breaking someone else's things.

Try:

* A Windows VM
* A Linux VM
* A small virtual network
* A web server
* A deliberately vulnerable application — [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) and [DVWA](https://github.com/digininja/DVWA) for web app bugs, [Metasploitable2](https://sourceforge.net/projects/metasploitable/) for OS and network-service bugs — both web apps are built around the [OWASP Top 10](https://owasp.org/www-project-top-ten/), the industry's own list of the most common and serious web vulnerability classes (SQL injection, cross-site scripting and the like). Worth a skim before diving in, so you recognise what you're actually looking at when you find something
* A logging system
* [Wireshark](https://www.wireshark.org) to actually watch the traffic your other lab machines are generating

!!! tip "Why you might see nothing in Wireshark"
    On a switched network, a device normally only sees traffic addressed to itself — not everything on the wire. To watch *other* devices' traffic on physical hardware, you need to configure a **SPAN port** (Cisco's term) or **monitor port** (most other vendors' term) on the switch, which mirrors another port's traffic to the one Wireshark is plugged into. Inside a virtual lab this is much simpler — most hypervisors let a VM's virtual network adapter run in "promiscuous mode," which does the same job without touching any physical switch config.

### A Windows and Active Directory lab

[Windows and Active Directory](foundations.md#windows-and-active-directory) is a common gap in self-taught learning, and it's genuinely worth lab time. Microsoft's own [Evaluation Center](https://www.microsoft.com/en-us/evalcenter) gives free, 180-day evaluation ISOs of Windows Server — enough to build a domain controller, promote it to a domain, then join a Windows client VM to it. Watching a login actually authenticate against a domain controller teaches you more about how AD works than reading about it ever will.

Then start experimenting.
