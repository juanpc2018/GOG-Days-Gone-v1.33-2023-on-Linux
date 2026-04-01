# GOG [Days Gone REMASTERED v1.33 (2023)](https://www.gog.com/en/game/days_gone) on Linux

GOG also has [DLC version](https://www.gog.com/en/game/days_gone_broken_road_dlc) "Paid Upgrade", and older v1.07 Original (2021) installer included with (2023). </br>

## Ubuntu 20.04.4 LTS

Lutris 0.5.18 is the most compatible .deb installer </br>
Lutris 0.5.20 .22 have "Special Requirements" *probably requires Ubuntu 24 or 25 </br>

The Goal is to Run Days Gone v1.33 as good as possible on Any Linux </br>
is 64-Bit but installing 32-Bit is required by Lutris. </br>

Days Gone v1.33 works on Ubuntu 20.04.4 LTS </br>
using System Wine 5, and System DXVK + Lutris .18 "Extra" Libraries, </br>
but has 4 fps </br>

Latest [WineHQ](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu), Linux Kernel & DXVK have: </br>
NTSync "perfect sync" between Linux Posix & Windows API calls "3rd gen sync" </br>
older Proton-ge / Wine & DXVK have Fsync "almost perfect" 2nd gen sync, </br>
E or N-sync "1st Gen Sync" </br>

Days Gone v1.33 REQUIRES some type of sync </br>
in Ubuntu 20.04.4 LTS Requires to compile a Newer DXVK v1.3.0 minimum </br>
Ubuntu 20.04.4 comes with: </br>
Kernel 5.15 </br>
Wine v5 </br>
DXVK 1.2 </br>

Optional: Liquorix Kernel 6.13 </br>

## Ubuntu 20.04.6 LTS

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 20.10

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 21.04

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 21.10

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 22.04.5 LTS "Jammy" & Linux Mint 21.x

Ubuntu 22.04.5 comes with: </br>
Kernel 6.8 </br>
Wine v6 </br>
DXVK 1.9 </br>

Optional Liquorix Kernel 6.19 Only works with NVIDIA driver 580 </br>
older nvidia drivers & dkms Do Not work with latest Liquorix Kernel in 22.04.5 </br>
but in 20.04.4 LTS does. </br>

Kernel 6.8 does Not work with Nvidia Driver 470 on 22.04.5 LTS, </br>
but Nvidia driver 535 works ok, with minor issues. </br>

#### Do Not install Optional Drivers & Updates from install .iso </br>
Iso Installer, downloads & install "different" / "manual" Nvidia drivers vs. Software & Updates Aditional Drivers </br>

Also Requires Mesa drivers, & Vulkan drivers </br>
installing some drivers crash Ubuntu-Desktop </br>
install 1-by-1 & rebbot. </br>

> cat /etc/os-release

> sudo mkdir -pm755 /etc/apt/keyrings
> wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo gpg --dearmor -o /etc/apt/keyrings/winehq-archive.key -

32-Bit
> sudo dpkg --add-architecture i386

> sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/jammy/winehq-jammy.sources
> sudo apt update

> sudo apt install --install-recommends winehq-stable
> sudo apt install --install-recommends winehq-staging
or
> sudo apt install --install-recommends winehq-devel

Ubuntu 22.04 KDE Neon reeport problems with: libpoppler-glib8 dependency. </br>
Solution: Downgrade package to official Ubuntu version: </br>
> sudo apt install libpoppler-glib8:{i386,amd64}=22.02.0-2ubuntu0.3 </br>

## Ubuntu 22.10

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>


## Ubuntu 23.04

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 23.10

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>

## Ubuntu 24.04 LTS

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>
