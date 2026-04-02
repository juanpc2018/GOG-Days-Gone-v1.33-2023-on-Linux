# GOG [Days Gone REMASTERED v1.33 (2023)](https://www.gog.com/en/game/days_gone) on Linux

GOG also has [DLC version](https://www.gog.com/en/game/days_gone_broken_road_dlc) "Paid Upgrade", and v1.07 "Original" (2021) installer included with (2023). </br>

## Ubuntu [20.04.4 LTS](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01)

Lutris [0.5.18](https://github.com/lutris/lutris/releases/tag/v0.5.18) is the most compatible .deb installer </br>
Lutris [0.5.20](https://github.com/lutris/lutris/releases/tag/v0.5.20) / [.22](https://github.com/lutris/lutris/releases/tag/v0.5.22) have "Special Requirements" *Ubuntu 24 or 25 </br>

The Goal is to Run Days Gone v1.33 as good as possible on Linux </br>
is 64-Bit but installing 32-Bit is required by Lutris. </br>

[Days Gone v1.33](https://www.gog.com/en/game/days_gone) works on Ubuntu [20.04.4 LTS](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01) </br>
using System Wine 5, and System DXVK + Lutris .18 "Extra" Libraries, </br>
but has [4 fps](https://www.reddit.com/r/linux_gaming/comments/nrz1wt/days_gone_with_winelutris_at_4fps/) </br>
"works" Lutris .18 forced to [1.7.1](https://github.com/doitsujin/dxvk/releases/tag/v1.7.1) Not Manual v1.2.13 </br>
very [low fps](https://github.com/doitsujin/dxvk/issues/2065) </br>
![Image](https://github.com/user-attachments/assets/093284b7-f13d-493b-9241-b6c252c0678a) </br>
Small Error: </br>
![Image](https://github.com/user-attachments/assets/36609f90-f7a3-4f4a-847f-4e97b82191e1) </br>

NVIDIA Driver 570 is the latest for Ubuntu [20.04.4 LTS](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01) </br>
NVIDIA Driver 470, Lutris Enable DXVK Complains is too old. </br>
but 20.04.4 LTS + NVIDIA 470 driver is required for Older 32-Bit games like Batman Arkham Asylum 32-Bit PhysX </br>
very old GPUs Quadro 6000 (2010) & GTX 470 Require driver 390 </br>

#### Sound
"PulseAudio" does Not work forced at 48KHz </br>
but Wine Config Test works ok. </br>
will test Jack later. </br>

Turning OFF DXVK, </br>
game works on newer Wine, </br>
but colors are wrong. </br>
speed fps also low = Worse. </br>

-----------------

## NTSync

Since: [WineHQ v10.16](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu), Proton-GE 10.9, Linux Kernel 6.14 (Mar"3"/2025) & DXVK, SteamOS 3.7.20 have: </br>
> $ ls -l /dev/[NTSync](https://www.youtube.com/watch?v=PFkX9wN8xPE&t=91s)

"perfect sync" between Linux Posix & Windows API calls "3rd gen sync" </br>
2019 Proton-ge "Wine" & DXVK have F-sync "almost perfect" 2nd gen sync, </br>
2018 E-sync "1st Gen Sync" </br>
Older: Wineserver NoSync </br>

[Days Gone v1.33](https://www.gog.com/en/game/days_gone) REQUIRES F-Sync or NTsync </br>
Ubuntu [20.04.4 LTS](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01) Requires to manually compile a Newer DXVK [v1.3.0](https://github.com/doitsujin/dxvk/releases/tag/v1.3) minimum </br>
Ubuntu 20.04.4 comes with: </br>
Kernel 5.15 </br>
wine-5.0 (Ubuntu 5.0-3ubuntu1) </br>
DXVK 1.2.13 </br>
mesa-vulkan 21.2.6 </br>
![Image](https://github.com/user-attachments/assets/6ab39365-c1ce-46f9-b180-0b82b48e4036)

Optional: Liquorix Kernel [6.3.13-1](https://github.com/damentz/liquorix-package/releases/tag/6.3-13) Tested on 20.04.4 LTS | [6.3-12](https://github.com/damentz/liquorix-package/releases/tag/6.3-12) -> [6.4.1](https://github.com/damentz/liquorix-package/releases/tag/6.4-1)  </br>
NTSync REQUIRES Kernel [6.14-1](https://github.com/damentz/liquorix-package/releases/tag/6.14-1) or Newer[-2](https://github.com/damentz/liquorix-package/releases/tag/6.14-2).[-3](https://github.com/damentz/liquorix-package/releases/tag/6.14-3).[-4](https://github.com/damentz/liquorix-package/releases/tag/6.14-4).[-5](https://github.com/damentz/liquorix-package/releases/tag/6.14-5).[-6](https://github.com/damentz/liquorix-package/releases/tag/6.14-6).[-7](https://github.com/damentz/liquorix-package/releases/tag/6.14-7).[-8](https://github.com/damentz/liquorix-package/releases/tag/6.14-8).[-9](https://github.com/damentz/liquorix-package/releases/tag/6.14-9).[-10](https://github.com/damentz/liquorix-package/releases/tag/6.14-10).[-11](https://github.com/damentz/liquorix-package/releases/tag/6.14-11).[-12](https://github.com/damentz/liquorix-package/releases/tag/6.14-12).[-13](https://github.com/damentz/liquorix-package/releases/tag/6.14-13).[-14](https://github.com/damentz/liquorix-package/releases/tag/6.14-14) </br>

## Ubuntu [20.04.6 LTS](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01)

has: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 20.10

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 21.04

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 21.10

comes with: </br>
Kernel 5. </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 22.04.5 LTS "Jammy" & Linux Mint 21.x

Ubuntu 22.04.5 comes with: </br>
Kernel 6.8 </br>
Wine v6 </br>
DXVK 1.9 </br>
mesa-vulkan </br>

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
mesa-vulkan </br>

## Ubuntu 23.04

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 23.10

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>

## Ubuntu 24.04 LTS

comes with: </br>
Kernel  </br>
Wine v </br>
DXVK 1. </br>
mesa-vulkan </br>
