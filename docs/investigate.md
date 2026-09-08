# Learn to Investigate

## OSINT — Open Source Intelligence

OSINT means finding and analysing information that's publicly available.

No hacking required.

It's used in threat intelligence, investigations, journalism, fraud detection and security research.

!!! danger "Before you start"
    Looking at publicly available information doesn't automatically mean you're entitled to use it however you want. Don't use OSINT to stalk, harass, impersonate or target people.

| Technique / Tool                                         | What it does                                                                       |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Google Lens / Reverse Image Search                       | Find where an image appears elsewhere online                                       |
| [TinEye](https://tineye.com)                             | Reverse image searching                                                            |
| [Sherlock](https://github.com/sherlock-project/sherlock) | Search for a username across many platforms                                        |
| [ExifTool](https://exiftool.org)                         | Examine metadata stored in files and images                                        |
| [GeoGuessr](https://geoguessr.com)                       | Useful practice for visual geolocation                                             |
| Google search operators                                  | Narrow searches using `site:`, `"exact phrase"`, `filetype:` and similar operators |

### Try this on yourself

Search your own name and usernames like a stranger would.

What can you find?

* Old accounts
* Old usernames
* Public photos
* Forgotten profiles
* Information you've posted publicly
* Things you didn't realise were visible

That's one of the best introductions to OSINT because you're investigating a target you are actually authorised to investigate:

**yourself.**

## Digital forensics basics

Where OSINT looks at what's public, digital forensics looks at what's already on a device — recovering, preserving and analysing evidence after something's happened. It's named as its own career direction in [Career Paths](career-paths.md), but hadn't actually been covered here until now.

| Tool                                                                        | What it does                                                                                    |
| ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| [Autopsy](https://www.autopsy.com)                                          | Free, open-source platform for analysing a disk image — files, timelines, deleted data              |
| [FTK Imager](https://www.exterro.com/digital-forensics-software/ftk-imager) | Free tool for creating a forensically sound copy of a drive before anyone analyses it — needs free registration to download |

The [golden rule](tools.md) applies here too: image and analyse your own drives, or a purpose-built forensic image someone's published for practice — never someone else's device without permission.

[CyberDefenders](https://cyberdefenders.org) has free, real-world DFIR challenges — actual disk images, memory dumps and packet captures to practise against once the tools are installed.

!!! info "This section is thin, and that's known"
    This is a starting point, not a real pathway — actively looking for someone with genuine DFIR experience to build it out properly. If that's you, [get in touch](https://github.com/t-d-knight/break-things-safely) — until then, treat this as "better than nothing," not "figured out."
