Other packages to include
https://www.kali.org/blog/kali-linux-metapackages/

---

# KALIPAK: Kali Linux Metapackage Installer CLI

This script was created to install Kali Linux metapackages on your Kali distribution. Information in this `README.md` file was taken from [kali.org](https://www.kali.org/docs/general-use/metapackages).

### What is a Metapackage?

Metapackages are used to install many packages at once, created as a list of dependencies on other packages. Kali Linux uses these in a few ways such as allowing users to decide how many packages out of the total Kali list they would like to install.

## Installing `kalipak`

It's recommended that `kalipak` be installed on `PATH` for optimal performance. These instructions will be the same for almost any script you want to install on a system.

### Windows

The recommended `PATH` directiory for KALIPAK is `C:\Windows\Scripts` or copy to `C:\Windows`.

1. The first step depends which version of Windows you have installed:
    - If you're using Windows 8 or 10, press the Windows key, then search for and
    select "System (Control Panel)".
    - If you're using Windows 7, right click the "Computer" icon on the desktop
    and click "Properties".
2. Click "Advanced system settings".
3. Click "Environment Variables".
4. Under "System Variables", find the `PATH` variable, select it, and click
   "Edit". If there is no `PATH` variable, click "New".
5. Add your directory to the beginning of the variable value followed by `;` (a
   semicolon). For example, if the value was `C:\Windows\System32`, change it to
   `C:\Windows\Scripts;C:\Windows\System32`.
6. Click "OK".
7. Restart your terminal.

### Mac OS X

1. Open the `.bash_profile` file in your home directory (for example,
   `/Users/your-user-name/.bash_profile`) in a text editor.
2. Add `export PATH="$PATH:kalipak-dir"` to the last line of the file, where
   *kalipak-dir* is the directory you want to add.
3. Save the `.bash_profile` file.
4. Restart your terminal.

### Linux

1. Open the `.bashrc` file in your home directory (for example,
   `/home/your-user-name/.bashrc`) in a text editor.
2. Add `export PATH=$PATH:kalipak-dir` to the last line of the file, where
   *kalipak-dir* is the directory you want to add.
3. Save the `.bashrc` file.
4. Restart your terminal.

## How to use

It's always good practice to update the package list before installing or upgrading existing packages because the system cannot know whether the repo has a new version of a package, unless it has an up-to-date copy of the package list.

You can manually update the package list with the following command or by selecting "Update" in the menu.

```
kalipak --update-pkg
```

Run `kalipak` from the terminal to enter the selection menu for installation.

```
KALIPAK: Kali Linux Metapackage Installer
https://www.kali.org/docs/general-use/metapackages
--------------------------
Select package to install:
1) System
2) Desktop
3) Hardware
4) Exploit
5) Extra
6) Update
7) Exit
#? 
```

## Usage

```
Usage: kalipak [--update-pkg] [--help] [--version]

Options:
  -i, --update-pkg    update package list and upgrade
  -h, --help          display this help and exit
  -v, --version       display version and exit
```

## Metapackage List [(kali.org)](https://www.kali.org/docs/general-use/metapackages)

### Kali System

- `kali-linux-core` - Base Kali Linux System – core items that are always included
- `kali-linux-headless` - Default install that doesn’t require GUI
- `kali-linux-default` - “Default” desktop (amd64/i386) images include these tools
- `kali-linux-arm` - All tools suitable for ARM devices
- `kali-linux-nethunter` - Tools used as part of Kali NetHunter

### Desktop environments/Window managers

- `kali-desktop-core` - Any key tools required for a GUI image
- `kali-desktop-e17` - Enlightenment (WM)
- `kali-desktop-gnome` - GNOME (DE)
- `kali-desktop-i3` - i3 (WM)
- `kali-desktop-kde` - KDE (DE)
- `kali-desktop-lxde` - LXDE (WM)
- `kali-desktop-mate` - MATE (DE)
- `kali-desktop-xfce` - Xfce (WM)

### Special Tools

- `kali-tools-gpu` - Tools which benefit from having access to GPU hardware
- `kali-tools-hardware` - Hardware hacking tools
- `kali-tools-crypto-stego` - Tools based around Cryptography & Steganography
- `kali-tools-fuzzing` - For fuzzing protocols
- `kali-tools-802-11` - 802.11 (Commonly known as “Wi-Fi”)
- `kali-tools-bluetooth` - For targeting Bluetooth devices
- `kali-tools-rfid` - Radio-Frequency IDentification tools
- `kali-tools-sdr` - Software-Defined Radio tools
- `kali-tools-voip` - Voice over IP tools
- `kali-tools-windows-resources` - Any resources which can be executed on a Windows hosts
- `kali-linux-labs` - Environments for learning and practising on

### Menu (Attacks, Exploits & Analysis)

- `kali-tools-information-gathering` - Used for Open Source Intelligence (OSINT) & information gathering
- `kali-tools-vulnerability` - Vulnerability assessments tools
- `kali-tools-web` - Designed doing web applications attacks
- `kali-tools-database` - Based around any database attacks
- `kali-tools-passwords` - Helpful for password cracking attacks – Online & offline
- `kali-tools-wireless` - All tools based around Wireless protocols – 802.11, Bluetooth, RFID & SDR
- `kali-tools-reverse-engineering` - For reverse engineering binaries
- `kali-tools-exploitation` - Commonly used for doing exploitation
- `kali-tools-social-engineering` - Aimed for doing social engineering techniques
- `kali-tools-sniffing-spoofing` - Any tools meant for sniffing & spoofing
- `kali-tools-post-exploitation` - Techniques for post exploitation stage
- `kali-tools-forensics` - Forensic tools – Live & Offline
- `kali-tools-reporting` - Reporting tools

### Extras

- `kali-linux-large` - Our previous default tools for amd64/i386 images
- `kali-linux-everything` - Every metapackage and tool listed here
- `kali-desktop-live` - Used during a live session when booted from the image

## License

KALIPAK is available under the MIT License. See [LICENSE](./LICENSE) for the full license text.



