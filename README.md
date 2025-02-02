# Wi-Fi Mangoapple Resources
Created this info-dump repo as an extension to my YouTube videos about the cheap DIY Wi-Fi Pineapple, AKA **Wi-Fi Mangoapple**. Hoping it helps people that have questions about supported chipsets, configurations, errors, etc..

*I'll keep updating this as much as possible. If you run into problems using this project, open up a GitHub Issue on the [main "Wi-Fi Prineapple Clone" project repo by xchwarze](https://github.com/xchwarze/wifi-pineapple-cloner).*

## Table of Contents
- [Guide Videos](https://github.com/SHUR1K-N/wifi-mangoapple-resources#guide-videos)
	- [Hardware & installation (easiest method)](https://github.com/SHUR1K-N/wifi-mangoapple-resources#hardware--installation-easiest-method)
	- [Upgrade + configuration, tips, chipsets, troubleshooting, and more](https://github.com/SHUR1K-N/wifi-mangoapple-resources#upgrade--configuration-tips-chipsets-troubleshooting-and-more)
- [Chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#chipsets)
  - [Notes](https://github.com/SHUR1K-N/wifi-mangoapple-resources#notes)
  - [2.4GHz / dual-band adapter decision](https://github.com/SHUR1K-N/wifi-mangoapple-resources#how-do-i-know-whether-i-should-get-a-24ghz-or-dual-band-adapter)
  - [Supported 2.4GHz chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#supported-24ghz-chipsets)
  - [Supported 2.4GHz + 5GHz (dual-band) chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#supported-24ghz--5ghz-dual-band-chipsets)
  - [Tested & confirmed as NOT supported](https://github.com/SHUR1K-N/wifi-mangoapple-resources#tested--confirmed-as-not-supported)
  - [Personally ordered RT5370 adapter links](https://github.com/SHUR1K-N/wifi-mangoapple-resources#personally-ordered--verified-rt5370-adapter-links-non-affiliate)
- [Troubleshooting](https://github.com/SHUR1K-N/wifi-mangoapple-resources#troubleshooting)
  - ["Status:Monitor interface won't start! Try to run airmon-ng..."](https://github.com/SHUR1K-N/wifi-mangoapple-resources#statusmonitor-interface-wont-start-try-to-run-airmon-ng-error-message)
  - [Can't connect to open AP](https://github.com/SHUR1K-N/wifi-mangoapple-resources#cant-connect-to-open-ap)

## Guide Videos
### Hardware & installation — easiest method
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/udnxagkSzoA/maxresdefault.jpg)](https://youtu.be/udnxagkSzoA)

### Upgrade + configuration, tips, chipsets, troubleshooting, and more
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/pHtpso21P0o/maxresdefault.jpg)](https://youtu.be/pHtpso21P0o)

---
---
# Chipsets
## Notes
* The Wi-Fi adapter discussed in my videos (RT5370 chipset) does _only_ 2.4GHz
* The Wi-Fi Mangoapple is capable of 5GHz sniffs & attacks as well if a 5GHz adapter with a _supported_ chipset is used instead of the RT5370; but I've not personally tested those

## How do I know whether I should get a 2.4GHz, or dual-band adapter?

Your selection of bands (2.4GHz or dual-band) would depend on the wireless awareness in your region/hood (in terms of security, adaptation to new technology, etc.).

Most *traditional* APs operate only on 2.4GHz.

Most *modern* APs are ″dual-band″ ― they operate on both 2.4GHz (for long range + smart home devices) and 5GHz (for higher speeds at short ranges).

The *latest* APs even go 6GHz (even higher speeds).

A good starting point to learning about wireless security―at least personally―would be 2.4GHz. But, of course, it would be best if you also tap into 5GHz since that has now become the new norm.

> TL;DR:
> 
> Dual-band = 2.4GHz + 5GHz
> 
> You'd be missing out on sniffs & attacks for APs and clients that are operating on the 5GHz band (5GHz channels)

## Supported 2.4GHz chipsets
As per documentation, some research, and comments on my videos:

* MT7603E/EN
* MT7620A/N
* MT7621
* MT7622
* MT7628
* RT2070 ― _not part of my research; mentioned by someone in the video comments_
* RT2400
* RT2500
* RT2570
* RT2671
* RT2770
* RT2870
* RT3070 ― _confirmed by someone in the video comments_
* RT3071
* RT3072
* RT3370
* RTL8187L/B
* RT5370 ― _personally confirmed + used in my Mangoapple videos_

## Supported 2.4GHz + 5GHz (dual-band) chipsets
As per documentation, some research, and comments on my videos:

* MT7632U
* MT7613
* MT7610U
* MT7662U/E
* MT7915
* RT3572 ― _confirmed by someone in this repo's Issues_
* RT5572 ― _personally confirmed + confirmed by someone in the video comments, Instagram, and Reddit_
* MT7612U ― _most problematic chipset. Try to stay away from it. In several adapters with this chipset, the adapter's **internal emulated storage** is recognized instead of the **Wi-Fi adapter** itself. If running "lsusb" shows the device ID as "0e8d:2870", then you're in that same boat (the "toast" boat). You should either look into another chipset, or get another adapter with the same chipset and try again, or there are multiple commands & configurations you could try to ″switch″ the adapter's mode from storage to Wi-Fi (but it may get tricky and is not worth it)_

## Tested & confirmed as NOT supported
As per documentation, some research, and comments on my videos:

* MT7610
* MT7601U
* AR9271
* RTL8811AU
* MT7921AUN

## Personally ordered & verified RT5370 adapter links (non-affiliate)
* https://a.aliexpress.com/_ooLUeiX (1 quantity order limit)
* https://a.aliexpress.com/_ooHxnUP

_If you find any more supported (or unsupported) chipsets during your testing, let me know in the Issues / Discussions / YouTube video comments. Many of us would benefit from your intel and appreciate it!_

---
---

# Troubleshooting
## "Status:Monitor interface won't start! Try to run airmon-ng..." error message
You're most likely using a Wi-Fi adapter with an _unsupported_ chipset. It's just a catch-all error message, and playing around with airmon-ng will not fix this. You'll need an adapter with a [supported chipset]().

## Can't connect to open AP
1. ″Filters″ page in the web UI
2. Switch both client and SSID filtering to ″Deny List″
3. "Networking" page, go to the "Config" tab
4. Ensure "Hide Open SSID" is _unchecked_
   > NOTE: the SSID _will_ be broadcasted sometimes even when set to hidden, so uncheck it regardless
6. "Update Access Point" button, regardless of the above setting
