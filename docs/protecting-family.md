# Protecting the Non-Technical People in Your Life From Scams

> This isn't a learning pathway. It's a shortlist of things you can actually install or set up for a parent, grandparent, or anyone else who isn't going to read a phishing awareness course but who you'd like to stop losing money to a stranger on the phone.
>
> Be upfront about cost where it isn't free. Nobody trusts a tool more for being oversold.

---

## If you only do one thing

Sit with them and turn on a password manager and MFA on their email account. Email is the recovery path for almost everything else — if it's compromised, everything downstream is exposed. The [Protect Yourself First](protect-yourself.md) page covers this in more detail.

---

## If it's free, work out who's paying for it

The old line "if you're not paying for the product, you're the product" undersells it slightly. It's not that *you're* the product — it's that your data is. Nobody runs a free VPN, a free "PC cleaner", or a free game out of charity. Something funds the servers and the developers, and if that something isn't a subscription fee, it's usually one of: selling browsing, location or contact data to advertisers and data brokers, running ads (sometimes disguised as "system alerts"), or a relentless upsell once someone's hooked.

This isn't a reason to avoid everything free — plenty of free software funds itself openly and reasonably, and several things on this page are exactly that. The difference is whether the business model is visible and makes sense, or whether it's a mystery.

**A quick test before installing anything free for a relative: could you explain, in one sentence, how this company makes money?** If the honest answer is "no idea," that's the signal to look elsewhere — not because free is automatically bad, but because an invisible business model usually means the data *is* the business model.

Worth connecting this back to the rest of this page: the data harvested by shady "free" software doesn't stay abstract. Email addresses, phone numbers and browsing habits sold through data broker pipelines are exactly the raw material scam operations buy to target people in the first place. A "free" app with a vague privacy policy isn't just a privacy inconvenience — it can be feeding the same pipeline this whole page exists to protect against.

---

## Purpose-built anti-scam software

| Tool | Cost | What it actually does |
| --- | --- | --- |
| [Seraph Secure](https://www.seraphsecure.com) | Free tier available; paid tier from ~US$4–6/mo (or ~US$14–21/mo covering up to 10 devices) | Built by scam-baiter Kitboga's team. The **free plan** (1 device, no account needed) removes existing remote-access tools and blocks new remote-connection attempts — that alone covers the single most damaging tech-support scam pattern. The **paid tier** adds the extras: blocking known scam websites, new-website and typo-squatting alerts, fake virus pop-up detection, and real-time alerts to a nominated family member. Used by some law enforcement agencies for scam forensics. The free tier is genuinely worth installing on its own; the paid tier is worth it for someone who's been targeted before or is a likely repeat target. |
| [Malwarebytes Browser Guard](https://www.malwarebytes.com/browserguard) | Free | Browser extension that blocks tech-support scam pop-ups, scam sites and malicious ads. Lighter-weight than Seraph Secure and doesn't need explaining — install it and forget it. |
| [uBlock Origin](https://ublockorigin.com) | Free | Ad blocker — and a lot of those fake "your PC is infected, call this number" pop-ups arrive via malicious ad networks in the first place, so blocking ads generally is blocking a scam delivery channel, not just a browsing-comfort feature. **Important nuance as of 2026:** the full, original uBlock Origin only still works properly on **Firefox**. Chrome forced out its old extension system this year, so Chrome (and Chromium browsers like Edge and Brave) now only support **uBlock Origin Lite**, a deliberately weaker version with far fewer filtering capabilities. If someone's on Chrome and you want them properly protected, either install uBlock Origin Lite and accept it's a lesser version, or — genuinely worth considering for a non-technical relative — just move them to Firefox, where the full version still works as well as it always has. |

## Endpoint protection — without a subscription

**For Windows: Microsoft Defender — the one already built in, not an app to install.** This is the genuinely good news. Independent testing through 2026 (AV-TEST, AV-Comparatives) has Defender scoring on par with paid suites for malware detection, with no bloat, no upsells, and nothing to buy. For most home users this is the correct, complete answer — there's no need to install anything else on top of it. Confirm it's switched on via Windows Security in Settings, keep Windows itself updated, and that's a solid baseline covered at zero cost. (This is the free one baked into Windows — different from the "Microsoft Defender for individuals" app mentioned below, which is the cross-platform one bundled with a paid Microsoft 365 subscription.)

**For Mac: the built-in XProtect and Gatekeeper cover most realistic day-to-day threats**, but "Macs don't get viruses" is less true than it used to be — Mac-specific infostealer malware (Atomic Stealer, Cuckoo Stealer) has grown noticeably. For most home users the built-in protection plus sensible habits (not installing cracked software, not disabling Gatekeeper to run something dodgy) is still enough. If someone wants a genuine no-subscription extra layer: **Malwarebytes Free** — but note the free tier is an on-demand scanner, not continuous real-time protection, so it's a "run it occasionally as a second opinion" tool rather than a full replacement for anything.

**One rule regardless of platform: run one real-time antivirus, not two.** Two real-time engines running at once fight each other for the same files and usually just slow the machine down rather than doubling the protection. An occasional on-demand scan (Malwarebytes Free) alongside whatever's running full-time is fine, since it's not continuously active — but don't install a second "always-on" antivirus over the top of Defender or XProtect.

The difference in scope: Seraph Secure is aimed squarely at the remote-access tech-support scam (the one where someone convinces a victim to install AnyDesk and hand over control of their PC) — and its free tier already covers that core case. Browser Guard is a broader but shallower net, and free across the board.

## Software worth actively avoiding

Grouping these together on purpose, because the pattern matters more than any single name. Most of what follows makes money the same way: convince a non-technical person their computer has a problem it doesn't have, then charge them to fix it.

**Consumer "security suites" — Avast, AVG, and the rest of that shelf.** This isn't just a reputation slip — it's ownership. Avast, AVG, Norton, LifeLock and Avira are all now the same company (Gen Digital). Avast in particular got caught selling users' detailed browsing data through a subsidiary called Jumpshot, and the aggressive upsell tactics that made the free versions annoying never really went away after the merger — they just spread across the whole family of brands. Picking a different name from that same shelf doesn't dodge the problem; it's largely one commercial approach wearing several logos. Use what's already built in instead (see above).

**Driver "optimizer" tools** (Driver Booster, DriverFix, Driver Support, and similar). These scan a PC and report a list of "outdated" drivers — sometimes accurately, often not — to sell an upgrade to the paid version. Windows Update already handles the overwhelming majority of driver needs on its own, and for the rare case it doesn't, going straight to the manufacturer's own site (Nvidia, AMD, Intel) is safer than a third-party tool that's occasionally installed an incompatible driver and broken something that wasn't broken to begin with.

**Registry cleaners and "PC optimizer" suites** (Advanced SystemCare, MyCleanPC, and the "your PC has 47 errors, click to fix" family). Modern Windows and macOS don't need registry or junk-file cleaning the way old advice used to suggest — at best these do nothing measurable, at worst they've been known to destabilise a system by "fixing" something that wasn't actually broken.

**MacKeeper — worth a specific, honest mention because it's a mixed case, not a clean avoid.** Its history is bad: a 2015 breach exposed 13 million users' data, and it built its reputation in the 2010s on fake "your Mac is infected" scareware pop-ups designed to frighten people into paying. Under different ownership since 2019, the current product is genuinely AV-TEST certified and no longer behaves like scareware. So if a relative already has it installed, it's not an emergency — but there's no compelling reason to seek it out over the free built-in tools above, and the marketing pattern that built its reputation is exactly the "urgency plus a scary warning" shape this whole page is trying to train people to notice.

**"Free" VPNs from an app store search.** A VPN costs real money to run — server infrastructure, bandwidth, maintenance. This is the "if it's free, work out who's paying for it" test from above, applied directly: if nobody's charging for a VPN and the business model isn't obvious, the honest answer is often "logging and selling exactly the browsing data a VPN is supposed to hide." Stick to a VPN attached to a company with a visible, sensible business model — the Google One VPN mentioned below is a good example of "free because it comes bundled with something you're already paying for," which is a different thing entirely from "free with no visible source of income."

**Bundled offers in installer windows.** The pattern to teach, not just the specific software: legitimate free installers (CCleaner, uTorrent, and plenty of others over the years) have made money by bundling in extra toolbars, browser hijackers, or trial security suites with a pre-checked box during install. Always choose "custom" or "advanced" install over "quick" install, and actually read what's pre-checked before clicking next.

## Already paying for it? Turn it on.

This is the highest-value section on this page. A lot of genuinely solid protection is sitting unused inside subscriptions people already pay for every month — nobody ever surfaces it to them.

| If they have... | They already get... | Worth knowing |
| --- | --- | --- |
| **Microsoft 365 Personal or Family** | **Microsoft Defender for individuals** — cross-platform malware protection (Windows, Mac, iOS, Android), a single security dashboard showing every family member's device status, and identity/dark-web monitoring | The identity and credit monitoring side is US-only, so it won't do much for an Australian household on that front — but the cross-device malware protection and family security dashboard work everywhere, and it's already paid for. No reason to also be running a separate "free" antivirus that nags for upgrades. |
| **iCloud+** (any paid iCloud tier) | **Hide My Email** (generates disposable forwarding addresses so their real email never goes to a sketchy signup form), **Private Relay** (encrypts Safari browsing traffic so their ISP or a shared wifi network can't see what they're visiting) | Both are already switched on for most people by default once they're on a paid tier — worth checking Settings → [name] → iCloud to confirm rather than assuming. |
| **Google One** (any tier, including the cheapest) | **VPN by Google One** — encrypts all device traffic, not just browser traffic, and is included on every plan tier including the AU$2-ish/month entry level | Google shut down its old "Dark Web Report" feature in February 2026, so don't go looking for it — it no longer exists. Google now points people to **Security Checkup** and **passkeys** instead, both free and worth setting up regardless of which ecosystem someone's in. |
| **Telstra, Optus, or another major Australian telco** | Network-level scam call and SMS filtering, already on by default | Neither carrier requires you to do anything — Telstra's "Cleaner Pipes" and Optus's "Call Stop" block scam calls and texts before they reach the phone, automatically, for every customer. Worth checking they haven't been accidentally opted out (Telstra: text `FILTER ON` to re-enable if it's ever been turned off) rather than telling someone to go install a third-party call-blocking app on top. |

The pattern across all of these: check what's already switched on before recommending something new. It's free, it's already trusted (they're already a customer), and it doesn't add "one more app" to a phone that's already confusing enough.

## Free, built-in options worth turning on

* **Windows Family Safety** / **Google Family Link** — free, allow a family member to see activity or get alerts on a relative's device. Feels intrusive for an adult, so use judgement about whether it's appropriate — this is really aimed at kids' devices.
* **Browser phishing/malware warnings** (Microsoft Defender SmartScreen, Safari's Fraudulent Website Warning, Chrome Safe Browsing) — on by default in most modern browsers, but worth checking they haven't been switched off.
* **Call screening / spam ID** — most Android phones and iPhones now have built-in spam call filtering, on top of whatever the telco is already blocking at the network level. Two layers is better than one.

## Government and non-profit resources (Australia)

* [Scamwatch](https://www.scamwatch.gov.au) — current scam alerts, reporting, and plain-English explanations of how specific scams work. Good to bookmark on a relative's computer.
* [Be Connected](https://beconnected.esafety.gov.au) — free digital literacy program aimed at older Australians, run by eSafety. Better pitched at someone who wants to build confidence with a computer generally, not just avoid scams.
* [IDCARE](https://www.idcare.org) — free support line if someone's already had identity or financial information compromised, not just a "might happen" concern.
* **Free credit report freeze** — Equifax, illion and Experian all let Australians place a free ban on new credit checks against their name. This doesn't cost anything and isn't tied to any subscription — worth doing after any scam involving personal details, or proactively for anyone who's a likely target (older relatives, anyone whose details have appeared in a data breach).

## Watch for government impersonation scams specifically

A large share of scams targeting older Australians impersonate the ATO, myGov, or Services Australia — a call or text claiming a tax debt, a Centrelink overpayment, or a myGov account "suspension" that needs urgent action. These work because they use real government branding and create exactly the urgency-plus-consequence pressure covered in the main pathway doc's [human side of security](protect-yourself.md) section. The ATO and Services Australia will never ask for payment via gift cards, cryptocurrency, or direct bank transfer to resolve a debt over the phone — that pattern alone is enough to hang up.

## The conversation matters more than the software

No tool replaces the one thing that actually stops most of these: telling the person, clearly and without lecturing them, that **nobody legitimate will ever ask them to install remote access software, buy gift cards, or move money urgently.** If they hear that once from someone they trust, before it happens, that's worth more than most of what's on this list.

If a scam does happen: see [If Something Actually Goes Wrong](if-something-goes-wrong.md) for what to do and who to report it to.
