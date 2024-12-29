# Lenovo-Thinkpad-L470-Opencore-EFI
Opencore EFI for installing Mac OS Big Sur on Lenovo Thinkpad L470



<img src="https://m.media-amazon.com/images/I/51TwKqhakhS.jpg" alt="Lenovo Thinkpad L470 image"/>

**Tested on Mac OS Big Sur**, Fully working + iServices.

Disclaimer: I'm not responsible for any damage you may cause, use this at your own risk (I Strongly recommend making your own EFI).

---

| My Specs:                                   |
|---------------------------------------------|
| Intel Core i5-6200u                         | 
| Intel HD 520 Graphics                       |
| 8GB DDR4 RAM (2133MHz)                      |
| 256GB SSD                                   |
| 1920x1080 14 inches                         |

Works with both configurable Intel Wifi Cards:
- Intel Dual Band Wireless-AC 8260, Wi-Fi 2x2 802.11ac + BT4.1, M.2 card
- Intel Dual Band Wireless-AC 8265, Wi-Fi 2x2 802.11ac + BT4.1, M.2 card

# How to use this?

After you've followed the guide on [how to make the installation media](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/), just download the folder in this repository, and copy it in the main directory of your installation media.

A Correctly formatted media, should contain *two folders* in its root:
- **"com.apple.recovery.boot"** - with the Mac OS "BaseSystem" or "RecoveryImage" file(s).
- **"EFI"** - The one you've downloaded from here.

If You want to also use iServices, you'll need to modify the "config.plist" file, located in EFI>OC>"config.plist", using the ["ProperTree"](https://github.com/corpnewt/ProperTree) editor.

After you've opened the file using ["ProperTree"](https://github.com/corpnewt/ProperTree), follow the  [dortania's guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#platforminfo) on how to use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and apply modifications.
___




## Tools I Used:
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
