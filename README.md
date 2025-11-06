# Wi-Fi Mangoapple Resources
Created this info-dump repo as an extension to my YouTube videos about the cheap DIY Wi-Fi Pineapple, AKA **Wi-Fi Mangoapple**. Hoping it helps people that have questions about supported chipsets, configurations, errors, etc..

*I'll keep updating this as much as possible. If you run into problems using this project, open up a GitHub Issue on the [main "Wi-Fi Prineapple Clone" project repo by xchwarze](https://github.com/xchwarze/wifi-pineapple-cloner).*

## Table of Contents
- [Guide Videos](https://github.com/SHUR1K-N/wifi-mangoapple-resources#guide-videos)
	- [Hardware & installation (easiest method)](https://github.com/SHUR1K-N/wifi-mangoapple-resources#hardware--installation-easiest-method)
	- [Upgrades, configuration, tips, chipsets, troubleshooting, and more](https://github.com/SHUR1K-N/wifi-mangoapple-resources#upgrade--configuration-tips-chipsets-troubleshooting-and-more)
- [Parts](https://github.com/SHUR1K-N/wifi-mangoapple-resources#parts)
	- [Base Wi-Fi Mangoapple](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#basic-wi-fi-mangoapple)
 	- [Upgraded Wi-Fi Mangoapple](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#upgraded-wi-fi-mangoapple)
- [Chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#chipsets)
  - [Notes](https://github.com/SHUR1K-N/wifi-mangoapple-resources#notes)
  - [2.4GHz / dual-band adapter decision](https://github.com/SHUR1K-N/wifi-mangoapple-resources#how-do-i-know-whether-i-should-get-a-24ghz-or-dual-band-adapter)
  - [Supported 2.4GHz chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#supported-24ghz-chipsets)
  - [Supported 2.4GHz + 5GHz (dual-band) chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#supported-24ghz--5ghz-dual-band-chipsets)
  - [Tested & confirmed as NOT supported](https://github.com/SHUR1K-N/wifi-mangoapple-resources#tested--confirmed-as-not-supported)
  - [Personally confirmed & cheapest adapter links](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#personally-ordered--verified-adapter-links-non-affiliate)
- [Community Cases & Mods](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#community-cases--mods)
  - [CASE - Mangoapple + 2 adapters + USB hub + power bank](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#case-wi-fi-mangoapple--2-adapters--usb-hub--power-bank)
  - [MOD - 4 USB ports + case](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#mod-4-usb-ports--case)
- [Troubleshooting](https://github.com/SHUR1K-N/wifi-mangoapple-resources#troubleshooting)
  - ["Status:Monitor interface won't start! Try to run airmon-ng..."](https://github.com/SHUR1K-N/wifi-mangoapple-resources#statusmonitor-interface-wont-start-try-to-run-airmon-ng-error-message)
  - [Can't connect to open AP](https://github.com/SHUR1K-N/wifi-mangoapple-resources#cant-connect-to-open-ap)
  - [OpenWRT v19.07.7 not available](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#openwrt-v19077-not-available-in-the-openwrt-firmware-selector)
  - [No handshakes captured](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#no-handshakes-captured)
  - [Can't format USB flash drive / USB flash drive unrecognized](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#cant-format-usb-flash-drive-or-usb-flash-drive-not-recognized)
  - [No ″Install to SD″ button for modules](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#no-install-to-sd-button-for-modules)
  - [Going back to stock firmware](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources#going-back-to-the-mangos-stock-firmware)

## Guide Videos
### Hardware & installation — easiest method
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/udnxagkSzoA/maxresdefault.jpg)](https://youtu.be/udnxagkSzoA)

### Upgrade + configuration, tips, chipsets, troubleshooting, and more
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/pHtpso21P0o/maxresdefault.jpg)](https://youtu.be/pHtpso21P0o)

---
---
# Parts
## Basic Wi-Fi Mangoapple
* GL.iNet Mango (v2) router ([Official](https://store.gl-inet.com/products/gl-mt300n-v2-mini-smart-router) / [Amazon](https://www.amazon.com/dp/B073TSK26W))
* 1× Wi-Fi adapter with a [supported chipset](https://github.com/SHUR1K-N/wifi-mangoapple-resources#chipsets)

## Upgraded Wi-Fi Mangoapple
* GL.iNet Mango (v2) router ([Official](https://store.gl-inet.com/products/gl-mt300n-v2-mini-smart-router) / [Amazon](https://amzn.to/4lEX3lK))
* 2× Wi-Fi adapters with [supported chipsets](https://github.com/SHUR1K-N/wifi-mangoapple-resources#chipsets)
* USB flash drive
* USB hub with a minimum of 3 ports [Amazon](https://amzn.to/4eHnm8r)

---
---
# Chipsets
## Notes
* The Wi-Fi adapter discussed in my videos (RT5370 chipset) does _only_ 2.4GHz
* The Wi-Fi Mangoapple is capable of 5GHz sniffs & attacks as well if a 5GHz adapter with a _supported_ chipset is used

## How do I know whether I should get a 2.4GHz, or dual-band adapter?

Your selection of bands (2.4GHz or dual-band) would depend on the wireless awareness in your region/hood (in terms of security, adaptation to new technology, etc.).

Most *traditional* APs operate only on 2.4GHz.

Most *modern* APs are ″dual-band″ ― they operate on both 2.4GHz (for long range + smart home devices) and 5GHz (for higher speeds at short ranges).

The *latest* APs even go 6GHz (even higher speeds).

A good starting point to learning about wireless security―at least personally―would be 2.4GHz. But, of course, it would be best if you also tap into 5GHz since that has now become the new norm.

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
* RT5370 ― _personally confirmed + used in my Mangoapple & Shadowapple videos_

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
* RTL8811AU/CU
* MT7921AUN

## Personally ordered & verified adapter links (non-affiliate)
### RT5370 (2.4GHz)
* https://www.aliexpress.com/item/2255799898010658.html (1 quantity order limit)
* https://www.aliexpress.com/item/2255799900873717.html
* https://www.aliexpress.com/item/1005008142040949.html ― _confirmed by someone on Patreon_

### RT5572 (dual-band)
* https://www.aliexpress.com/item/3256806000755742.html
* https://www.aliexpress.com/item/1005008392078147.html ― _confirmed by someone on Instagram_
* https://www.aliexpress.com/item/1005009223339345.html ― _confirmed by someone on Patreon_

_If you find any more supported (or unsupported) chipsets during your testing, let me know in the Issues / Discussions / YouTube video comments. Many of us would benefit from your intel and appreciate it!_

---
---

# Community Cases & Mods
## [CASE] Wi-Fi Mangoapple + 2 adapters + USB hub + power bank

![large_display_IMG_0600](https://github.com/user-attachments/assets/e6b36dc4-31ee-4643-b4dd-139424c0267b)

[Thingiverse page with .STLs](https://www.thingiverse.com/thing:6939373)

## [MOD] 4 USB ports + case

![hub1](https://github.com/user-attachments/assets/9afa54da-3d45-49d3-ad47-e63a79f2dc1a)

[.STL file here](https://github.com/SHUR1K-N/WiFi-Mangoapple-Resources/blob/main/mods/4%20USB%20ports/case.stl)

---
---

# Troubleshooting
## "Status:Monitor interface won't start! Try to run airmon-ng..." error message
You're most likely using a Wi-Fi adapter with an _unsupported_ chipset. It's just a catch-all error message. Playing around with airmon-ng will not fix this. You'll need an adapter with a [supported chipset](https://github.com/SHUR1K-N/wifi-mangoapple-resources#chipsets).

## Can't connect to open AP
1. ″Filters″ page in the web UI
2. Switch both client and SSID filtering to ″Deny List″
3. "Networking" page, go to the "Config" tab
4. Ensure "Hide Open SSID" is _unchecked_
   > NOTE: the SSID _will_ be broadcasted sometimes even when set to hidden, so uncheck it regardless
6. "Update Access Point" button, regardless of the above setting

## OpenWRT v19.07.7 not available in the OpenWRT firmware selector
OpenWRT v19.07.7 seems to have been deprecated lately. You can use OpenWRT v21.02.0-rc2 instead, and follow the same steps as in the [tutorial video](https://github.com/SHUR1K-N/wifi-mangoapple-resources#hardware--installation-easiest-method).

> The only difference in the process: While flashing the Pineapple clone image via OpenWRT, _deselect_ the "Keep settings..." option and _select_ the "Force upgrade" option

> NOTE: If v21.02.0-rc2 is unavailable in the future as well, you can use my backup copy (`openwrt-21.02.0-rc2-ramips-mt76x8-glinet_gl-mt300n-v2-squashfs-sysupgrade.bin` in this repo)

> NOTE: OpenWRT v21.02.0-rc2, as far as I've tested, doesn't seem to have any observable issues that weren't already present with v19.07.7

## No handshakes captured
Though the handshakes are not *shown* in the web UI, they're actually being saved at root (/). The normal behavior would be saving handshakes in the handshakes directory (/tmp/handshakes).

The above ″misplacing″ of handshakes seems to be a problem with the project itself (at least for some people). The project author has a [GitHub Issue open](https://github.com/xchwarze/wifi-pineapple-cloner/issues/57) for this as well.

One ″workaround″ I've found very recently is using a router with the mips_24kc architecture like the GL.iNet AR300M-16 (Shadow). Can confirm, handshakes are shown in the web UI using that router.

## Can't format USB flash drive OR USB flash drive not recognized
1. Verify the USB flash drive is OK by checking it out on your Windows machine first
2. Try manually formatting the USB flash drive (Windows defaults are OK)
3. Re-attach it and see if it gets picked up correctly (″USB & Storage″ section on the ″Advanced″ page of the web UI should show you the model), or you could run ″lsusb″ / ″lsblk″ manually via SSH
4. If it's picked up, try running `wpc-tools format_sd` again (from *outside* the /sd/ directory)
5. If none of the above works, run the following commands:
   
   `opkg update`
   
   `opkg install kmod-usb-storage-uas`
7. Try running `wpc-tools format_sd` again (from *outside* the /sd/ directory)
8. If none of this works, try another USB flash drive altogether (multiple people have reported this fixed it)

## No ″Install to SD″ button for modules
1. Re-install missing packages using `wpc-tools missing_packages`

## Going back to the Mango's stock firmware
1. Get to the recovery mode again (as shown in the video)
2. Flash the [original router firmware](https://dl.gl-inet.com/router/mt300n-v2/stable)
