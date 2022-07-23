# KALIPAK: Kali Linux Metapackage Installer CLI

This script was created to install Kali Linux metapackages on your Kali disrtribution. Information in this `README.md` file was taken from [kali.org](https://www.kali.org/docs/general-use/metapackages).

### What is a Metapackage?
Metapackages are used to install many packages at one time, created as a list of dependencies on other packages. Kali Linux uses these in a few ways. One way is allowing users to decide how many packages out of the total Kali list they would like to install. Need just enough to use Linux? Want enough to conduct Pentests? Perhaps nearly every package available in Kali?

## Running the script

Run `kalipak` from the terminal to enter the selection menu for installation.

```
KALIPAK: Kali Linux Metapackage Installer
https://www.kali.org/docs/general-use/metapackages
------------------------
Select tools to install:
1) System
2) Desktop
3) Hardware
4) Exploit
5) Others
6) Exit
#? 
```

## Usage

```
Usage: kalipak [--help|--version]
-h, --help      display this help and exit
-v, --version   display version and exit
```

## Metapackage List [(kali.org)](https://www.kali.org/docs/general-use/metapackages)
### System

- `kali-linux-core` -  Base Kali Linux System – core items that are always included
- `kali-linux-headless` -  Default install that doesn’t require GUI
- `kali-linux-default` -  “Default” desktop (amd64/i386) images include these tools
- `kali-linux-arm` -  All tools suitable for ARM devices
- `kali-linux-nethunter` -  Tools used as part of Kali NetHunter

### Desktop environments/Window managers

- `kali-desktop-core` -  Any key tools required for a GUI image
- `kali-desktop-e17` -  Enlightenment (WM)
- `kali-desktop-gnome` -  GNOME (DE)
- `kali-desktop-i3` -  i3 (WM)
- `kali-desktop-kde` -  KDE (DE)
- `kali-desktop-lxde` -  LXDE (WM)
- `kali-desktop-mate` -  MATE (DE)
- `kali-desktop-xfce` -  Xfce (WM)

### Tools
- `kali-tools-gpu` -  Tools which benefit from having access to GPU hardware
- `kali-tools-hardware` -  Hardware hacking tools
- `kali-tools-crypto-stego` -  Tools based around Cryptography & Steganography
- `kali-tools-fuzzing` -  For fuzzing protocols
- `kali-tools-802-11` -  802.11 (Commonly known as “Wi-Fi”)
- `kali-tools-bluetooth` -  For targeting Bluetooth devices
- `kali-tools-rfid` -  Radio-Frequency IDentification tools
- `kali-tools-sdr` -  Software-Defined Radio tools
- `kali-tools-voip` -  Voice over IP tools
- `kali-tools-windows-resources` -  Any resources which can be executed on a Windows hosts
- `kali-linux-labs` -  Environments for learning and practising on

### Menu (Attack/Exploit)

- `kali-tools-information-gathering` -  Used for Open Source Intelligence (OSINT) & information gathering
- `kali-tools-vulnerability` -  Vulnerability assessments tools
- `kali-tools-web` -  Designed doing web applications attacks
- `kali-tools-database` -  Based around any database attacks
- `kali-tools-passwords` -  Helpful for password cracking attacks – Online & offline
- `kali-tools-wireless` -  All tools based around Wireless protocols – 802.11, Bluetooth, RFID & SDR
- `kali-tools-reverse-engineering` -  For reverse engineering binaries
- `kali-tools-exploitation` -  Commonly used for doing exploitation
- `kali-tools-social-engineering` -  Aimed for doing social engineering techniques
- `kali-tools-sniffing-spoofing` -  Any tools meant for sniffing & spoofing
- `kali-tools-post-exploitation` -  Techniques for post exploitation stage
- `kali-tools-forensics` -  Forensic tools – Live & Offline
- `kali-tools-reporting` -  Reporting tools

### Others

- `kali-linux-large` -  Our previous default tools for amd64/i386 images
- `kali-linux-everything` -  Every metapackage and tool listed here
- `kali-desktop-live` -  Used during a live session when booted from the image

## License

KALIPAK is available under the <ins>MIT License</ins>. See [LICENSE](./LICENSE) for the full license text.
