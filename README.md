# nextdns-settings

My recommendations for the ultimate NextDNS Configuration :)

**NOTE:** This project can be found on both [Codeberg](https://codeberg.org/Magnesium1062/nextdns-settings), which will act as the main & preferred way to contribute, and [GitHub](https://github.com/Retold3202/nextdns-settings).

# Security

**Use Threat Intelligence Feeds** -> ✅

**Enable AI-Driven Threat Detection** -> ✅

**Enable Google Safe Browsing** -> ✅ **Even with this setting, you should still ENABLE Safe Browsing in your browser. This list is limited exclusively to domains, while browser Safe Browsing can also check downloaded files.**

**Enable Cryptojacking Protection** -> ✅

**Enable DNS Rebinding Protection** -> ✅

**Enable IDN Homograph Attacks Protection** -> ✅

**Enable Typosquatting Protection** -> ✅

**Enable DGA Protection** -> ✅

**Block Newly Registered Domains (NRDs)** -> ✅ *(This will cause very rare breakage, but massively improves security)*

**Block Dynamic DNS Hostnames** -> ✅

**Block Parked Domains** -> ✅

**Block Top-Level Domains (TLDs)** -> 

I would recommend taking a look at blocking TLDs from HaGeZi's "Most Abused TLDs" list [here](https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/spam-tlds.txt). Block whatever works best for you. This can be tedious, but does a lot to heavily reduce risk of malicious websites. *(I've seen this work in real-time, blocking scam/spam domains before they were picked up by any lists)*.

**Block Child Sexual Abuse Material** -> ✅ *(Apologies to the pedos in the audience...)*

# Privacy

**Blocklists** ->

Here's where it gets fun.

Despite popular opinion, due to the reasons WaLLy3K has listed [here](https://github.com/WaLLy3K/wally3k.github.io?tab=readme-ov-file#why-use-this-over-other-sources), I think it's a good idea to use multiple lists and sources, rather than just limiting yourself to one or two giant lists. I myself constantly notice domains being blocked that were caught by only one or two lists and missed by others. **I'm not saying you should go overboard, but I do think it's a good idea to use a variety of high quality lists for the best coverage possible.**

I would generally recommend using the following:

* ⭐️ `AdAway`

* ⭐️ `AdGuard DNS filter`

* ⭐️ `Anudeep's Blacklist for ads and trackers`

* ⭐️ `CAMELEON`

* ⭐️ `EasyList`

* ⭐️ `EasyPrivacy`

* ⭐️ `Fanboy's Annoyance List`

* ⭐️ `HaGeZi Multi Pro++`

* ⭐️ `hBlock`

* ⭐️ `hostsVN`

* ⭐️ `Lightswitch05 - Ads & Tracking`

* ⭐️ `NextDNS Ads & Trackers Blocklist` *(Enabled by default)*

* ⭐️ `NSABlocklist`

* ⭐️ `OISD`

* ⭐️ `Perflyst's Smart-TV Blocklist`

* ⭐️ `Personal Blocklist by WaLLy3K`

* ⭐️ `Peter Lowe`

* ⭐️ `someonewhocares.org (Dan Pollock)`

* ⭐️ `Steven Black`

* ⭐️ `WindowsSpyBlocker (Spy)`

It might seem like a lot, but these are high quality lists with strong coverage and minimal false positives in my experience, and it generally doesn't hurt to use them like this.

Additionally, if you're fine with a little breakage, I would highly recommend:

* ❓ `1Hosts `**(Pro)** 

* ❓ `HaGeZi - Multi `**Ultimate** instead of `HaGeZi Multi `**Pro++**

* ❓ `No Facebook` - *(Obviously don't use if you use any Facebook services)*

<br>

**Native Tracking Protection** ->

I would recommend enabling the following **in addition** to any devices you have that are listed:

* ⭐️ `Windows` *(Blocks Microsoft trackers, not exclusive to Windows)*

* ⭐️ `Amazon Alexa` *(Blocks Amazon trackers, not exclusive to Alexa)*

<br>

**Block Disguised Third-Party Trackers** -> ✅

**Allow Affiliate & Tracking Links** -> ✅ (See `Denylist` section below)

# Parental Control

**Websites, Apps & Games** -> You should use this feature to your advantage and block any services that you don't use or care about. This can dramatically improve your privacy by preventing connections to them from even being made. If you use a service, don't block it, just block what you're comfortable with and works best for you.

I usually block the following:

* `TikTok`

* `Snapchat`

* `Facebook`

* `Instagram`

* `VK`

* `Messenger`

* `WhatsApp`

* `Spotify`

# Denylist

Remember how we allowed affiliate & tracking links above?

While this is nice from a usability perspective, this does also allow some questionable ad/tracking domains that we don't want unblocked. I would recommend taking a look at [the allowlist NextDNS is using](https://github.com/nextdns/click-tracking-domains/blob/main/domains) and I would definitely add the following to your denylist:

* `ad.doubleclick.net`
* `adclick.g.doubleclick.net`
* The google adservice domain from the list corresponding to your region/that you run into
* `adservice.google.com`
* `amazon-adsystem.com`
* `analytics.twitter.com`
* `app.adjust.com`
* `dart.l.doubleclick.net`
* `pagead.l.doubleclick.net`
* `www.googleadservices.com`

Note that I maintain a variety of comprehensive blocklists [here](https://codeberg.org/Magnesium1062/BadBlock). Sadly you won't be able to add them to NextDNS, but you may skim through them and manually block whatever you wish to.

# Allowlist

Note that I maintain a comprehensive whitelist [here](https://codeberg.org/Magnesium1062/BadBlock/raw/branch/main/whitelist.txt). Sadly you won't be able to add it to NextDNS, but you may skim through it and manually allow whatever you wish to.

Regardless, you should allow the following for updates on Fedora Linux:

* `mirror.arizona.edu` # Blocked by NSABlocklist

You should also always allow `nextdns.io`, as this will ensure we can always access the dashboard, regardless of any rogue filters or unexpected events that could occur.

# Settings

**Enable Logs** -> ✅ *(Having logs on is important for troubleshooting breakage)*

**Log clients IPs** -> ❌

**Log domains** -> ✅

**Retention** -> `1 hour` *(This will allow us to easily troubleshoot breakage, without keeping data for longer than necessary)*

**Storage location** -> `Switzerland`

**Enable Block Page** -> ❌ *(⚠️ Please **NEVER** enable this. This causes lots of issues and weird breakage, and also heavily reduces security through compromising HTTPS)*

**Enable Anonymized EDNS Client Subnet** -> ❌ 

**Enable Cache Boost** -> ✅

**Enable CNAME Flattening** -> ✅

**Enable Web3** -> ❌ *if you don't use/need it*

# Account *(Select your email address in the top right corner)*

**Two-Factor Authentication (2FA)** -> ✅

# Additional recommendations

* Use a privacy-respecting browser like [Firefox](https://www.mozilla.org/firefox/) with a user.js like [Arkenfox](https://github.com/arkenfox/user.js).

* Make sure to configure NextDNS on **both** your OS and in your browser. This will allow you to take advantage of [Encrypted Client Hello](https://blog.cloudflare.com/announcing-encrypted-client-hello).

* Use a content blocking extension like [uBlock Origin](https://github.com/gorhill/uBlock). *(See recommended settings [here](https://codeberg.org/Magnesium1062/ublock-origin-settings))*

* Enable Safe Browsing in your browser if possible and if it's not done in a privacy-invasive way. (You should use i.e. [Google Safe Browsing on "Standard" Mode](https://safebrowsing.google.com/), [Firefox's Safe Browsing](https://support.mozilla.org/kb/how-does-phishing-and-malware-protection-work), [Brave's Safe Browsing](https://brave.com/privacy/browser/#safe-browsing), & [Safari's Fraudulent Website Warning](https://www.apple.com/legal/privacy/data/en/safari/), you should avoid most other options i.e. [Google Safe Browsing on "Enhanced" Mode](https://safebrowsing.google.com/), [Microsoft SmartScreen](https://learn.microsoft.com/windows/security/operating-system-security/virus-and-threat-protection/microsoft-defender-smartscreen/), & [Opera Sitecheck](https://blogs.opera.com/security/2021/01/making-browsing-safe-from-phishing/)).

* Use a (reputable) anti-virus if possible. On Windows, you can use the built-in [Microsoft Defender Antivirus](https://en.wikipedia.org/wiki/Microsoft_Defender_Antivirus), on macOS, you can stick to the built-in [XProtect](https://support.apple.com/guide/security/protecting-against-malware-sec469d47bd8/web), on Android, you can use [Hypatia](https://f-droid.org/packages/us.spotco.malwarescanner/), and on Linux, you can use [ClamAV](https://www.clamav.net/). **NOTE:** You should install Hypatia through the [DivestOS Official Repo](https://divestos.org/fdroid/official/?fingerprint=E4BE8D6ABFA4D9D4FEEF03CDDA7FF62A73FD64B75566F6DD4E5E577550BE8467) instead of F-Droid's main repo, as it will allow you to receive quicker updates directly from the developer. It's also recommended to use [F-Droid Basic](https://f-droid.org/en/packages/org.fdroid.basic/) as your F-Droid client of choice.