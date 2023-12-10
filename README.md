# How to Popbuntu?
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/themagicalmammal/howtopopbuntu/blob/master/LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-blue.svg)](https://github.com/themagicalmammal/howtopopbuntu/graphs/commit-activity)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-blue.svg?style=flat)](https://github.com/themagicalmammal/howtopopbuntu/pulls)

This is an extensive Guide on the set of things I use.

Changed some stuff and deleted others to better fit my use case.

# Index

## [Post Installation](#1-post-installation)
- **[Update your System](#update-your-system)**
- **[Gnome Tweaks & the ones I use](#gnome-tweaks--the-ones-i-use) -> [Minimize Button and Button Placement](#1-minimize-button-and-button-placement), [Battery Percentage](#2-battery-percentage), [Optimizing Font](#3-optimizing-font), [Activity Hot Corner](#4-activity-hot-corner-and-format-time)**

## [Preferred Apps](#2-preferred-apps)
- **[Snap Vs Flatpak](#snap-vs-flatpak-package-managers-except-apt-dpkg)**
- **[Browser](#browser) -> [Firefox](#1-firefox), [Extensions](#extensions-i-use)**
- **[Email Client](#email-client)->  [MailSpring](#3-mailspring)**
- **[Video Tools](#video-tools) -> [VLC](#1-vlc), [OBS Studio](#2-obs-studio), [Peek](#3-peek)**
- **[Audio Tools](#audio-tools) -> [PulseAudio Controls](#1-pulseaudio-controls), [PulseEffects](#2-pulseeffects), [Audacity](#3-audacity)**
- **[Office](#office) -> [Libre Office](#1-libreoffice)**
- **[Social Apps](#social-apps) -> [Telegram](#1-telegram), [Discord](#2-discord)**
- **[Programming Apps](#programming-apps) -> [Vim](#1-vim), [GitHub-Desktop](#3-github-desktop), [Visual Studio](#5-visual-studio)**
- **[Entertainment Apps](#entertainment-apps) -> [Spotify](#1-spotify-for-music), [Steam](#2-steam-for-gaming), [Multimedia Codecs](#3-multimedia-codecs), [Lutris](#4-lutris)**
- **[Other Apps](#other-apps) ->  [Wine](#2-wine-windows-apps), [Synaptic](#3-synaptic-package-manager), [Nautilus](#4-nautilus-admin-mode), [Timeshift](#5-timeshift), [Resource Monitor](#6-resource-monitor), [Firewall](#7-firewall)**
- **[Debloat](#--debloat)**

## [Optimize Boot-time & Ram Usage](#3-optimize-boot-time--ram-usage)
- **[Disabling Plymouth](#disabling-plymouth)**
- **[Adjusting the Swappiness Property](#adjusting-the-swappiness-property)**
- **[Adjusting the Cache Pressure](#adjusting--the-cache-pressure-setting)**
- **[Disable Pop Shop on boot](#disabling-pop-shop-on-boot)**
- **[Clearing buff/cache](#clearing-buffcache)**
- **[Optimizing the boot](#optimizing-the-boot)**
- **[Custom Kernel](#custom-kernel)**
- **[Removing Custom Kernel](#getting-rid-of-custom-kernel)**
- **[Final Boot-Time](#final-boot-time)**

## [Miscellaneous](#4-miscellaneous)
- **[Terminal Mods](#terminal-mods) -> [Neofetch](#1-neofetch), [Shell Config](#2-shell-config)**
- **[TLP](#tlp)**
- **[Disable Frequents](#disable-frequents)**
- **[Clean your System](#clean-your-system)**
- **[Night Light](#night-light)**
- **[Tile Windows](#tile-windows)**
- **[Custom Fonts](#custom-fonts)**
- **[Customization](#customization)**

## [Inspiration](#Inspiration)

## 1. Post Installation
These are some of the things I do after a fresh install of PopOs.

### Update the system
*Get the latest updates via terminal or some GUI based updater or Apps stores(like Pop shop).* <br />
In my case I mainly update my system through the terminal, so i use the commands:
```bash
sudo apt update && sudo apt upgrade -y && flatpak update
```
For Forced update
```bash
sudo apt install -f && sudo apt dist-upgrade
```
### Updating your recovery (Pop Os)
If you upgrade to a newer release the recovery also needs to be upgraded, you can do it via Terminal. <br />
```bash
pop-upgrade recovery upgrade from-release
```

### Gnome Tweaks & the ones I use
```bash
sudo apt install gnome-tweaks -y
```

#### 1. Minimize Button and Button Placement
Restores the minimize and the maximize button.
#### 2. Battery Percentage
Shows the amount of battery remaining in percent. Doesn't work for desktop pc.
#### 3. Activity Hot Corner and Format time
The activity hot corner enables the hot corner where the button Activity is placed. So rather than clicking the button just touch the edge.

## 2. Preferred Apps
Pop has apps that you need. But, if you do not like them, you can also get alternatives. <br />
### Snap Vs Flatpak (Package Managers except apt, dpkg)
Snap can incorporate more apps than Flatpak. It runs how the developer wants it to. Some even say go as far as to say, "Snap is the future". But, currently, Flatpak outperforms Snap, for the most part, that is why I don't prefer Snap but, still, it's your choice. <br />
### Browser
#### 1. [Firefox](https://www.mozilla.org/en-US/firefox/new/)
The Browser that I use in any of my setups is always Firefox, and it's an amazing browser, it helps that I am currently trying to take anything related to Google out of my setups. <br />
By default Firefox comes pre installed in any of the distros I tried so you don't need to install anything. <br />

#### Useful Extensions
Generally, these extensions exist for almost all browsers. <br />

1. [**uBlock Origin**](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) - uBlock Origin is not an "ad blocker", it's a wide-spectrum content blocker with CPU and memory efficiency as a primary feature.

2. [**ClearURLs**](https://addons.mozilla.org/pt-PT/firefox/addon/clearurls/) - ClearURLs removes any tracking elements from URLs.

3. [**HTTPS Everywhere**](https://addons.mozilla.org/pt-PT/firefox/addon/https-everywhere/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=recommended) - Encrypt the web! HTTPS Everywhere is a Firefox extension to protect your communications by enabling HTTPS encryption automatically on sites that are known to support it, even when you type URLs or follow links that omit the https: prefix.

4. [**LocalCDN**](https://addons.mozilla.org/pt-PT/firefox/addon/localcdn-fork-of-decentraleyes/) - Emulates remote frameworks (e.g. jQuery, Bootstrap, AngularJS) and delivers them as local resource. Prevents unnecessary 3rd party requests to Google, StackPath, MaxCDN and more. Prepared rules for uBlock Origin/uMatrix.

5. [**WebP image converter**](https://addons.mozilla.org/pt-PT/firefox/addon/webp-image-converter/) - I use this one because some times when I'm downloading any pictures sometimes it will save them as .webp, and in the case that happens I use this eextension and I can save in .png or .jpg.

6. [**GNOME Shell integration**](https://addons.mozilla.org/en-US/firefox/addon/gnome-shell-integration/) - This extension provides integration with GNOME Shell and the corresponding extensions repository, make it easy to add extensions via your browser.

7. [**Reddit Enhancement Suite**](https://addons.mozilla.org/pt-PT/firefox/addon/reddit-enhancement-suite/) - I'm an avid user of reddit, but I dislike the new look and use the old reddit and with this extension comes an amazing amount of features that can enhance your Reddit experience.

### Email Client
Currently as my email client I use Mailspring.
[MailSpring](https://getmailspring.com/)
Get the [deb file](https://github.com/Foundry376/Mailspring/releases) and try installing it. <br />
If it throws gvfs dependency error. Follow these **Steps:**
1. Install these libraries
```bash
sudo apt install libsecret-1-dev gconf2 python2 python-is-python2 -y
```
2. Install the deb,
```bash
sudo dpkg --ignore-depends=gvfs-bin -i mailspring*.deb
```

**If you want to remove Geary**
```bash
sudo apt-get autoremove --purge geary* -y
```

### Video Tools
#### 1. [VLC](https://www.videolan.org/index.html)
VLC is the best video player for any platform
```bash
sudo apt install vlc  -y
```

Get rid of the stock video player
```bash
sudo apt-get autoremove --purge totem* -y
```
#### 2. [OBS Studio](https://obsproject.com/)
OBS Studio is software designed for capturing, compositing, encoding, recording, and streaming video content, efficiently.
```bash
sudo apt install obs-studio -y
```

#### 3. [Peek](https://github.com/phw/peek)
Peek is an recorder with with video recording, GIF recording and screenshot capabilities. <br />
**Pop users don't need to add this repo.**
```bash
sudo add-apt-repository ppa:peek-developers/stable && sudo apt update
sudo apt install peek -y
```

### Audio Tools
#### 1. [PulseAudio Controls](https://www.freedesktop.org/wiki/Software/PulseAudio/)
PulseAudio is an audio server. The audio in your apps passes through Pulse. So in that way, you can use several methods to handle these sounds ere you can hear them. It also optimizes the quality of your audio.
```bash
sudo apt install pavucontrol -y
```
To learn how to control your audio, go [here](controlling-audio-devices).
#### 2. [PulseEffects](https://github.com/wwmm/pulseeffects)
Audio effects for Pulseaudio applications. This helps add specialized effects for each application individually and thus creates multiple profiles for different applications.
```bash
sudo apt install pulseeffects -y
```
**This might add a lot of desktop icons.**<br />
#### 3. [Audacity](https://www.audacityteam.org/)
Audacity is open-source software, easy-to-use, multi-track audio editor, and allows users to record audio and edit music clips.
```bash
flatpak install org.audacityteam.Audacity -y
```
#### 4. [Ardour](https://ardour.org/)
Ardour is a recorder and digital audio workstation app. It's made to be suitable for professional use.
```bash
sudo apt install ardour -y


### Office
I use LibreOffice as my Office suite.
```bash
sudo apt install libreoffice-gnome libreoffice
```
<br /> <br />

### Social Apps
#### 1. Telegram
Official Telegram client
```bash
flatpak install org.telegram.desktop -y
```
#### 2. Discord
Official Discord client
```bash
flatpak install com.discordapp.Discord -y
```

### Programming Apps
#### 1. Vim
```bash
sudo apt install vim
```
#### 3. GitHub-Desktop
A seamless way to contribute to projects on GitHub.
```bash
sudo apt install git github-desktop -y
```
If this doesn't work, get the deb [here](https://github.com/shiftkey/desktop/releases).

#### 5. Visual Studio
Go through [this](https://code.visualstudio.com/docs/setup/linux).

### Entertainment Apps
#### 1. Spotify for Music
**Supports Ad-block and Spicetify-cli**
```bash
curl -sS https://download.spotify.com/debian/pubkey_0D811D58.gpg | sudo apt-key add -
echo "deb http://repository.spotify.com stable non-free" | sudo tee /etc/apt/sources.list.d/spotify.list
sudo apt update && sudo apt install spotify-client -y
```
Features that can be added, <br />
##### 1. Spicetify-Cli & Themes

I use the this scripts to install [themagicalmammal/howtopopbuntu] (https://github.com/themagicalmammal/howtopopbuntu)

To install themes for spotify, you can check [this](https://github.com/khanhas/spicetify-cli), to install different themes, go [here](https://github.com/morpheusthewhite/spicetify-themes) out. If you have troubles going through the steps of spicetify-cli. Here is a script you can use.
```bash
curl -fsSL https://raw.githubusercontent.com/themagicalmammal/howtopopbuntu/master/spicetify.sh | bash
```
You need to log-in & out after this. <br />

#### 2. Steam for Gaming
```bash
sudo apt install steam -y
```
If it doesn't work, turn on multiverse.
```bash
sudo add-apt-repository multiverse && sudo apt update
```

I also use [Glorious Eggroll] (https://github.com/GloriousEggroll/proton-ge-custom) build of proton.

#### 3. Multimedia Codecs
Gives you the ability to play popular non-free media formats, including DVD, MP3, Quicktime and Windows Media.
```bash
sudo apt install ubuntu-restricted-extras -y
```
To enable restricted codecs to play DVDs
```bash
sudo apt install libdvd-pkg -y
sudo dpkg-reconfigure libdvd-pkg
```
#### 4. Lutris

Lutris is an Open Source gaming platform for Linux. It installs and launches games so you can start playing without the hassle of setting up your games. Get your games from GOG, Steam, Battle.net, Origin, Uplay and many other sources running on any Linux powered gaming machine. 

```bash 
sudo add-apt-repository ppa:lutris-team/lutris
sudo apt update
sudo apt install lutris
```

### Other Apps

#### 2. Wine (Windows Apps)
Wine (originally an acronym for "Wine Is Not an Emulator") is a compatibility layer capable of running Windows applications.
**Remove Wine if you have it installed**
1. If you have a 64-bit system this command will enable 32-bit support
```bash
sudo dpkg --add-architecture i386
```
2. Then follow these **Steps:**
```bash
wget https://dl.winehq.org/wine-builds/winehq.key && sudo apt-key add winehq.key
sudo apt-add-repository deb\ https://dl.winehq.org/wine-builds/ubuntu/\ $(lsb_release -c | sed 's/Codename:\t/''/g')\ main && sudo apt update
sudo apt install --install-recommends winehq-stable -y
```
3. Then open wine configuration, add download the additional wine files
```bash
winecfg
```
**Saftey with Wine** - Never use wine with sudo. Windows apps always run with admin rights in wine. No sudo needed sometimes, You need to tell wine to start an app as a "normal user" but, you never need to run it with admin rights because it already does. So from this, you could be thinking can't hurt to run wine with sudo, Right? Yes, it can hurt, or do you believe that a potential Virus wouldn't be happy to be run with root rights? Viruses work through wine like they would on Windows. sudo gives them even more privileges. <br />

#### 3. Synaptic Package manager
Synaptic serves as a graphical front-end to APT which makes the process of software management easier.
```bash
sudo apt install synaptic -y
```
#### 4. Nautilus (admin mode)
Adds right-click property *Open as Administrator*
```bash
sudo apt install nautilus-admin -y && nautilus -q
```
#### 5. Timeshift
Timeshift is a system restore tool for Linux. Creates a file system snapshot using rsync+hard links or BTRFS snapshots.
```bash
sudo apt install timeshift -y
```
#### 6. Bashtop
An advanced utility that shows usage and stats for processor, memory, disks, network, and processes.
**Repo already exists in Pop 20.10**
```bash
sudo add-apt-repository ppa:bashtop-monitor/bashtop && sudo apt update
sudo apt install bashtop -y
```
#### 7. Firewall
#### - Gufw
GUFW is a graphical utility for managing Uncomplicated Firewall (UFW). This is pretty easy to use appication with bunch of settings which you can set according to your preference.
```bash
sudo apt install gufw
```
### - Debloat
###### Remove useless stuff that you do not need.  Please, read what it does before you remove them.
- **Calculator** - You know what a calculator is.
```bash
sudo apt remove --purge gnome-calculator -y
```
- **Calendar** - I put this on a list because I never need the Calendar even on my phone
```bash
sudo apt autoremove --purge gnome-calendar -y
```
- **Character Map** - is a Unicode character map that allows you to select characters from a table and insert them into a text string. I have no known use for it.
```bash
sudo apt-get autoremove --purge gucharmap* -y
```
- **Contacts** - Gnome contacts tool important for a work pc.
```bash
sudo apt-get autoremove --purge gnome-contacts* -y
```
- **Document Scanner** - Important tool for a work pc.
```bash
sudo apt-get remove --purge sane* simple-scan -y
```
- **Gnome Fonts** - shows you the fonts installed on your computer for your use as thumbnails. Selecting any thumbnails shows the full view of how the font would look under various sizes.
```bash
sudo apt remove --purge gnome-font-viewer -y
```
- **Gnome Help** - Useful for newcomers
```bash
sudo apt-get autoremove --purge yelp* -y
```
- **Gnome Power Manager** - can show historical and current battery information and programs waking up that use power. I never use it.
```bash
sudo apt remove --purge gnome-power-manager -y
```
- **Pinyin (Only for Chinese users)** - Pinyin is the Romanization of Chinese characters based on their pronunciation.
```bash
sudo apt autoremove --purge ibus-libpinyin -y
```
- **Popsicle USB creator** - If you create a live USB, you should keep this tool but, Etcher seems a better option.<br />
**Get [Etcher](https://www.balena.io/etcher/)** <br />
```bash
sudo apt-get remove --purge popsicle* -y
```

#### Reverting
If you accidentally remove any, you can add them back by
```bash
sudo apt install <appname> -y
```
*App name doesn't require * symbol*

## 3. Optimize Boot-time & Ram Usage

My original boot-time was around 2min after removing apps it's now 42sec.<br /> <br />

### Disabling Plymouth
**For Pop OS** <br />
```bash
sudo kernelstub --delete-options "quiet systemd.show_status=false splash"
```
### Adjusting the Swappiness Property
This is required to adjust swap usage. If you have huge rams like 16GB ram then you can reduce this value to as low as 0. But if you have low ram devices like 1GB you should make this 90 or higher. Interactions with the swap file are costlier since swaps are slower than RAMs and they can cause a reduction in performance. <br />

Values according to me for Ram: Ratio should be as follows, 32:0, 16:10, 8:20, 4:50, 2:70 <br />
**20 is just an example value, don't mindlessly use it** <br />
```bash
sudo sysctl vm.swappiness=20
```
**These values do not stick. To add them permanently. Add the above line to sysctl.conf.** <br />
```bash
sudo nano /etc/sysctl.conf
```

### Adjusting  the Cache Pressure Setting
Another issue, the system stores cache about stuff that you frequently open & this makes the system faster, as if it opens again, rather than reloading the data it will use the cache. But, on a lower ram device, this is a bad option since this will seriously slow your system down. <br />
Adjust this like you adjusted swappiness property, values for RAM: Pressure should be as follows, 1:100, 2:90, 4:80, 8:60, 16:50.
```bash
sudo sysctl vm.vfs_cache_pressure=50
```
**Add the above line to sysctl.conf.** <br />
```bash
sudo nano /etc/sysctl.conf
```
### Disabling Pop Shop on Boot
Pop Shop always opens on the startup of the system there is a way to stop that. This also helps in saving some ram. <br /> <br />
**Steps:**
1. Edit App center daemon from opening it at start
```bash
sudo nano /usr/share/applications/io.elementary.appcenter-daemon.desktop
```
2. Put # here before this line
```bash
Exec=io.elemantry.appcenter -s
```
### Clearing buff/cache
The computer accumulates high buff/cache over time and makes the user force reboot. To clear buff cache, you can use this. <br />
```bash
free -h && sudo sysctl -w vm.drop_caches=3 && sudo sync && echo 3 | sudo tee /proc/sys/vm/drop_caches && free -h
```
### Optimizing the boot
#### DISCLAIMER
##### PLEASE DO THIS AT YOUR OWN RISK. WHILE THIS IS SAFE TO DO YOU CAN STILL MESS UP YOUR SYSTEM SO, PLEASE READ THIS CAREFULLY AND UNDERSTAND EVERYTHING BEFORE YOU PROCEED.
- **Network-dispatcher** is a dispatcher daemon for systemd-networkd connection status changes.
```bash
sudo apt remove --purge networkd-dispatcher -y
```
- **ModemManager** is a DBus-activated daemon that controls mobile broadband (2G/3G/4G) interfaces. If you do not have a mobile broadband interface, you do not need this.
```bash
sudo systemctl disable ModemManager.service
sudo systemctl mask ModemManager.service
```
**Note:** - If you are not using this and don't want Wi-Fi to disable wpa_supplicant.service.
- **fwupd** is a simple daemon allowing you to update some devices' firmware, including UEFI for several machines
Disable thunderbolt_power <br />
```bash
sudo nano /etc/fwupd/daemon.conf
```
Make it
```bash
BlacklistPlugins=test;invalid;thunderbolt_power
```
-[blacklist_thunderbold](https://github.com/themagicalmammal/howtopopbuntu/blob/master/References/blacklist_thunderbold.png)
Remove fwupd from boot
```bash
sudo systemctl disable fwupd.service
sudo systemctl mask fwupd.service
```
- **Avahi-daemon** is supposed to provide zero-configuration network discovery and make it super-easy to find printers and other hosts on your network. I always disable it and do not miss it.
```bash
sudo systemctl disable avahi-daemon.service
sudo systemctl mask avahi-daemon.service
```
- **Apport** collects potentially sensitive data, such as core dumps, stack traces, and log files. They can contain passwords, credit card numbers, serial numbers, and other private material.
```bash
sudo systemctl disable apport.service
sudo systemctl mask apport.service
```
- **Saned** is the SANE (Scanner Access Now Easy) daemon that allows remote
clients to access image acquisition devices available on the localhost.
```bash
sudo systemctl disable saned.service
sudo systemctl mask saned.service
```
- **GPU-Manager** is software that creates a xorg.conf for you. So running this in every boot is just overkill. You only need to run this if you change your GPU.
```bash
sudo systemctl disable gpu-manager.service
sudo systemctl mask gpu-manager.service
```
- **Apt-daily-upgrade** solves long boot up time with apt-daily-upgrade.
```bash
sudo systemctl disable apt-daily.service
sudo systemctl disable apt-daily.timer
sudo systemctl disable apt-daily-upgrade.timer
sudo systemctl disable apt-daily-upgrade.service
```
- **lvm2-monitor** Only useful if you are using lvm.
```bash
sudo systemctl disable lvm2-monitor.service
sudo systemctl mask lvm2-monitor.service
```
- **Systemd-resolved** [Restart Required]  is a system service that provides network name resolution to local applications. It implements a caching and validating DNS/DNSSEC stub resolver.
1. Disable & Mask the systemd-resolved service
```bash
sudo systemctl stop systemd-resolved.service
sudo systemctl disable systemd-resolved.service
sudo systemctl mask systemd-resolved.service
```
2. Then put dns=default in the [main] section of
```bash
sudo nano /etc/NetworkManager/NetworkManager.conf
```
3. Delete the symlink /etc/resolv.conf
```bash
sudo rm /etc/resolv.conf
```
4. Restart <br /> <br />

**Enable them back** <br />
Let the service name be xyz.service
```bash
sudo systemctl unmask xyz.service
sudo systemctl enable xyz.service
```
### Custom kernel
Custom Kernels are known and used by fewer people, but these kernels add a significant boost to performance and battery.
1. **Xanmod** is the more popular choice among intel based hardware. It provides a stable, responsive, and smooth desktop experience. <br />
To get Xanmod, go [here](https://xanmod.org/)  <br />
While installing this don't forget to add, **Setting the FQ-PIE Queuing Discipline**. <br />

2. **Liquorix** is a distro kernel replacement built using the best configuration and kernel sources for desktop, multimedia, and gaming workloads. Works better with AMD hardware. <br />
To get Liquorix, go [here](https://liquorix.net/) <br /> <br />

### Getting rid of Custom Kernel
**IF YOU ARE A NEW USER AND DON'T KNOW WHAT YOU ARE DOING, PLEASE SEARCH SOME THREADS OR ASK SOMEONE BEFORE TAKING ANY ACTION. BECAUSE THIS IS A VERY RISKY STEP AND CAN POTENTIALLY KILL YOUR SYSTEM.**<br />
1. Removing the Kernel apt modules <br />

For XanMod
```bash
sudo apt autoremove --purge linux-xanmod -y
```

For Liquorix
```bash
sudo apt autoremove --purge linux-image-liquorix-amd64 linux-headers-liquorix-amd64 -y
```
2. [XanMod Only] Remove FQ-PIE Queue Discipline for systemd
```bash
sudo rm /etc/sysctl.d/90-override.conf
```
4. Removing  the Kernel Repos <br />

For XanMod <br />
Download this [deb](https://dl.xanmod.org/xanmod-repository.deb) and uninstall it. <br />

For Liquorix <br />
```bash
sudo add-apt-repository -r ppa:damentz/liquorix
```
**Tip: -r can be after or before the repo, so you can also write,**
```bash
sudo add-apt-repository ppa:damentz/liquorix -r
```

5. Getting, name of the Kernel
```bash
uname -r
```
6. Removing the Kernel
```bash
sudo apt remove <kernel name> -y
```
7. Getting, remaining Kernel files
```bash
apt list --installed *xanmod* *liquorix*
```
8. Removing the remaining Kernel files
```bash
sudo apt remove <name of kernel files> -y
```

[Reference of installing and removing XanMod](https://www.reddit.com/r/pop_os/comments/jlrney/psa_installing_and_removing_the_xanmod_kernel_in/) <br />


## 6. Miscellaneous
### Terminal Mods
#### 1. [Macchina](https://crates.io/crates/macchina)

Macchina can be installed with cargo, to install cargo simply run:
```
sudo apt install cargo
```
Then:
```
cargo install macchina
```

![macchina](https://gitlab.com/Shoto31/popos-setup/-/raw/master/images/d.png)

#### 2. Shell Config 
I'm currently using the [Spaceship prompt](https://github.com/denysdovhan/spaceship-prompt)

### TLP
TLP is a utility for battery optimization on laptops. TLP comes with a default configuration which is perfectly tuned. The utility works by optimizing the power used by hardware devices while your laptop is running on its battery.
```bash
sudo apt install tlp
sudo tlp start
```
If you need a graphical interface to optimise or control it.
```bash
sudo add-apt-repository ppa:linuxuprising/apps && sudo apt update
sudo apt install tlpui
```

### Disable Frequents
Disable Frequents Tab in Gnome app menu. This option is not required for Gnome > 3.38.
```bash
gsettings set org.gnome.desktop.privacy remember-app-usage false

```
### Clean your System
#### Clean via Terminal
```bash
sudo apt --purge autoremove
sudo rm -rf ~/.cache/thumbnails/*
sudo apt clean
sudo apt autoclean
```

### Night Light
Night Light mode is simply made to remove some lights which hinder our sleep cycle. As researchers have found that at night if a certain set of colors interact with our eyes it doesn't let the eye rest making it *unsleepy* that's why we use a night light.<br /> <br />

### Tile Windows
In my setups I always use the Tile windows feature.

### Customization
#### 1. We need to add gnome-shell-integration for Firefox.
[Gnome Shell Extension](https://addons.mozilla.org/pt-PT/firefox/addon/gnome-shell-integration/)

#### 2. Then go to [Gnome.org](https://extensions.gnome.org/) and get your extensions. <br />
#### Important Extensions
- [User themes](https://extensions.gnome.org/extension/19/user-themes/)
- [Impatience](https://extensions.gnome.org/extension/277/impatience/) <br /> <br />
#### Some More Cool Extensions that I use.
- [Caffeine](https://extensions.gnome.org/extension/517/caffeine/) - Prevents your pc from going to sleep.

- [Coverflow Alt-Tab](https://extensions.gnome.org/extension/97/coverflow-alt-tab/) - Replacement of Alt-Tab, iterates through windows in a cover-flow manner.

- [Dash to Panel](https://extensions.gnome.org/extension/1160/dash-to-panel/)  <br /> <br />

![dashtopanel](https://gitlab.com/Shoto31/popos-setup/-/raw/master/images/2021-03-11_12-29.png)
To get the start button I [have](https://github.com/themagicalmammal/howtopopbuntu/blob/master/References/start.png). <br />

- [Panel OSD](https://extensions.gnome.org/extension/708/panel-osd/) - Configuring where on the (main) screen notifications will appear, instead of just above the message tray.

- [Status Area Horizontal Spacing ](https://extensions.gnome.org/extension/355/status-area-horizontal-spacing/) - Reduce the horizontal spacing between icons in the top-right status area.

-  [Vitals](https://extensions.gnome.org/extension/1460/vitals/) - A glimpse into your computer's temperature, voltage, fan speed, memory usage, processor load, system resources, network speed and storage stats.

## Inspiration
I decided to do this as a guide mainly for myself,  since I always forget some tweaks, extensions or applications, but my inspiracion was [The Magical Mammal/How to popbuntu] (https://github.com/themagicalmammal/howtopopbuntu#6-resource-monitor) you can check his for a more detailed guide.

## Discussion
To post suggestions or ask questions. Go to [Discussions](https://github.com/themagicalmammal/howtopopbuntu/discussions).

## Thanks for Suggestions
1. [GGG_246](https://www.reddit.com/user/GGG_246/) - A lot of stuff I didn't know. To check what he did go [here](https://www.reddit.com/r/Ubuntu/comments/jm1gvw/a_guide_to_setting_up_popubuntu/gasmuhg?utm_source=share&utm_medium=web2x&context=3) & [here](https://www.reddit.com/r/Ubuntu/comments/jm1gvw/a_guide_to_setting_up_popubuntu/gata2s4?utm_source=share&utm_medium=web2x&context=3) & a looooot more stuff.
2. [schykle](https://www.reddit.com/user/schykle) - Mailspring (fix for dangerous gvfs-bin bug) & Ubiquity auto Swap & GUI updater & Updated Snap instructions.
3. [wsadES](https://www.reddit.com/user/wsades) - Suggestion about removing unnecessary extension & Pop Shop on boot.
4. [tur1ngb0x](https://github.com/tur1ngb0x) - For qt5 theme fix & new wine installation steps.
5. [coolwyou](https://www.reddit.com/user/coolwyou) - For the awesome neofetch config file & shell config.
6. [spxak1](https://www.reddit.com/user/spxak1/) - Mention Firefox & Chromium-based Bug & Idea about Disclaimer & Reverting back to stock kernel.
7. [JawadAlkassim](https://www.reddit.com/user/JawadAlkassim/) - Mention opensource & Vivaldi vaapi & Wayland.
8. [arsfeld](https://www.reddit.com/user/arsfeld) - Information about Encryption and recovery.
9. [lulzdoods](https://www.reddit.com/user/lulzdoods) - Completing the uninstall guide for the kernel.
10. [RiderExMachina](https://www.reddit.com/user/RiderExMachina/) - Check out what he said [here](https://www.reddit.com/r/linux4noobs/comments/jqyi1c/want_to_switch_to_ubuntubased_distros_need_a/gbqvrbf?utm_source=share&utm_medium=web2x&context=3)
11. [1ntr0v3rt3ch](https://www.reddit.com/user/1ntr0v3rt3ch) - For steps for making a swap file.
12. [rbmorse](https://www.reddit.com/user/rbmorse/) - Practices on a swap.
