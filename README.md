## Hero Number One

What is Hero Number One?  
This is a modification for Serious Sam Classic The Second Encounter.   
This mod required https://github.com/tx00100xt/SeriousSamClassic or https://github.com/tx00100xt/SeriousSamClassic-VK to run.  
Hero Number One was created by fans of the game Serious Sam TSE and is distributed for free.    

Description: (From the authors of mod)  
In 2013, among the ruins of an ancient Mayan city, the remains of a refuge of an unknown cult were found, which disappeared long ago under unknown circumstances. The best experts in the world were engaged in the mystery, but no one could explain the origin of the oldest walls and columns made of extraterrestrial stone with carved panoramas of incredible fantastic worlds... When archaeologists unearthed another artifact, it turned out to be a portal from which hordes of terrible, beautiful, and simply amazing creatures poured out. In order to deter the invasion of creatures, special forces strike groups are landing in the archaeological complex with one goal - to destroy all witnesses and fill the complex with concrete... The work was masterfully done, but one of the archaeologists managed to survive...  
Trying to escape, he jumped into the portal...    

Author:  
ST-TEAM is author this mod for windows.

![HNO2](https://raw.githubusercontent.com/tx00100xt/SE1-TSE-HNO/main/Images/hno-2.png)

![HNO3](https://raw.githubusercontent.com/tx00100xt/SE1-TSE-HNO/main/Images/hno-3.png)


Download [HeroNumberOne.tar.xz] archive and unpack to  SeriousSamClassic/SamTSE/ directory.
To start the modification, use the game menu - item Modification.

Building Serious Sam Hero Number One (only for SS:TSE)
------------------------------------------------------

### Linux

Type this in your terminal:

```
git clone https://github.com/tx00100xt/SE1-TSE-HNO.git
cd SE1-TSE-HNO/Sources
./build-linux64.sh      	# use build-linux32.sh for 32-bits
```
After that , libraries will be collected in the x32 or x64 directory . Copy them to SeriousSamClassic/SamTSE/Mods/HNO/Bin folder.

### Gentoo

To build a game for gentoo, use a https://github.com/tx00100xt/serioussam-overlay containing ready-made ebuilds for building the game and add-ons.

### Arch Linux

To build a game under Arch Linux you can use the package from AUR: https://aur.archlinux.org/packages/serioussam

### Raspberry Pi

The build for raspberry pi is similar to the build for Linux, you just need to add an additional build key.

```
cd SE1-TSE-HNO/Sources
./build-linux64.sh -DRPI4=TRUE	# use build-linux32.sh for 32-bits
```
### FreeBSD

Install bash. 
Type this in your terminal:

```
git clone https://github.com/tx00100xt/SE1-TSE-HNO.git
cd SE1-TSE-HNO/Sources
bash build-linux64.sh      	# use build-linux32.sh for 32-bits
```
After that , libraries will be collected in the x32 or x64 directory . Copy them to SeriousSamClassic/SamTSE/Mods/HNO/Bin folder.

Windows
-------
* This project can be compiled starting from Windows 7 and higher.

1. Download and Install [Visual Studio 2015 Community Edition] or higher.
2. Download and Install [Windows 10 SDK 10.0.14393.795] or other.
3. Open the solution in the Sources folder, select Release x64 or Release Win32 and compile it.

Supported Architectures
----------------------
* `x86`
* `aarch64`
* `e2k` (elbrus)

Supported OS
-----------
* `Linux`
* `FreeBSD`
* `Windows`
* `Raspberry PI OS`

License
-------

* Serious Engine v1.10 is licensed under the GNU GPL v2 (see LICENSE file).


[HeroNumberOne.tar.xz]: https://drive.google.com/file/d/1Cxmzm8dk1WzaYS7vfzvzeILS8O78SC92/view?usp=sharing "Serious Sam Classic HeroNumberOne Mod"
[Visual Studio 2015 Community Edition]: https://go.microsoft.com/fwlink/?LinkId=615448&clcid=0x409 "Visual Studio 2015 Community Edition"
[Windows 10 SDK 10.0.14393.795]: https://go.microsoft.com/fwlink/p/?LinkId=838916 "Windows 10 SDK 10.0.14393.795"
