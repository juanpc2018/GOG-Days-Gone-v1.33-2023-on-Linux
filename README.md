# GOG Days Gone REMASTERED v1.33 (2023) on Linux

GOG also has DLC version "Paid Upgrade", and Free older v1.07 Original (2021) installers </br>

## Ubuntu 20.04.4 LTS

Lutris 0.5.18 is most compatible .deb installer </br>
Lutris 0.5.20 .22 have "Special Requirements" *probably requires Ubuntu 24 or 25 </br>

The Goal is to Run Days Gone v1.33 as good as possible on Any Linux </br>
Days gone is 64-Bit but installing 32-Bit is also a good idea. </br>

Days Gone v1.33 works on Ubuntu 20.04.4 LTS </br>
using System Wine 5, and System DXVK + Lutris "Extra" Libraries, </br>
but has 4 fps </br>

Latest [WineHQ](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu), Linux Kernel & DXVK have NTSync "perfect sync" between Linux & Windows API calls </br>
older Wine & DXVK have Fsync "almost perfect", E or N-sync </br>

Days Gone v1.33 REQUIRES some type of sync </br>
to make it work in Ubuntu 20.04.4 LTS requires to compile a Newer DXVK 1.3.0 minimum </br>
Ubuntu 20.04.4 comes with: </br>
Kernel 5.15 </br>
Wine v5 </br>
DXVK 1.2 </br>

## Ubuntu 22.04.5 LTS "Jammy" & Linux Mint 21.x

Ubuntu 22.04.5 comes with: </br>
Kernel 6.8 </br>
Wine v6 </br>
DXVK 1.9 </br>

Optional Liquorix Kernel 6.19 Only works with NVIDIA driver 580 </br>
older nvidia drivers & dkms Do Not work with latest Liquorix Kernel in 22.04.5 </br>
but in 20.04.4 LTS does. </br>

#### Do Not install Optional Drivers from install .iso </br>
Iso Installer, downloads & install "different" / "manual" Nvidia drivers version vs. Software & Updates Aditional Drivers </br>

Also Requires Mesa drivers, & Vulkan drivers </br>
installing some drivers can crash Ubuntu-Desktop </br>

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

Ubuntu 22.04 KDE Neon reeport problems with: libpoppler-glib8 dependency. 
Solution is to downgrade package to the official Ubuntu version:
> sudo apt install libpoppler-glib8:{i386,amd64}=22.02.0-2ubuntu0.3


