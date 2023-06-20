## Hero Number One
![Build status](https://github.com/tx00100xt/SE1-TSE-HNO/actions/workflows/cibuild.yml/badge.svg)
[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/tx00100xt/SE1-TSE-HNO)

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
You can also download the archive using curl or wget:
```
wget https://archive.org/download/hero-number-one/HeroNumberOne.tar.xz
wget https://archive.org/download/hno-data-messages-eng/HNO-Data-messages-eng.tar.xz
```
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

### Ubuntu

Instead of building you can install packages from ppa by adding ppa:tx00100xt/serioussam to your system's Software Sources.
```bash
sudo add-apt-repository ppa:tx00100xt/serioussam
sudo add-apt-repository ppa:tx00100xt/serioussam-mods
sudo apt update
```
This PPA can be added to your system manually by copying the lines below and adding them to your system's software sources.
```
deb https://ppa.launchpadcontent.net/tx00100xt/serioussam/ubuntu YOUR_UBUNTU_VERSION_HERE main 
deb-src https://ppa.launchpadcontent.net/tx00100xt/serioussam/ubuntu YOUR_UBUNTU_VERSION_HERE main 
```
After adding ppa, run the commands:
```bash
sudo apt install serioussamclassic serioussam-hno
```
or
```bash
sudo apt install serioussamclassic-vk serioussam-hno
```

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


### macOS

Install dependes
```
brew install bison flex sdl2 libogg libvorbis zlib-ng cmake git
```
Type this in your terminal:
```
git clone https://github.com/tx00100xt/SE1-TSE-HNO.git
cd SE1-TSE-HNO/Sources
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make -j4
make install
```
After that , libraries will be collected in the Mods directory.   
Copy them to SeriousSamClassic/SamTSE/Mods/HNO/Bin folder.

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
* `macOS`

### Build status
|CI|Platform|Compiler|Configurations|Platforms|Status|
|---|---|---|---|---|---|
|GitHub Actions|Windows, Ubuntu, FreeBSD, Alpine, Raspberry PI OS Lite, macOS|MSVC, GCC, Clang|Release|x86, x64, armv7l, aarch64, riscv64, ppc64le, s390x|![GitHub Actions Build Status](https://github.com/tx00100xt/SE1-TSE-HNO/actions/workflows/cibuild.yml/badge.svg)

You can download a the automatically build based on the latest commit.  
To do this, go to the [Actions tab], select the top workflows, and then Artifacts.

License
-------

* Serious Engine v1.10 is licensed under the GNU GPL v2 (see LICENSE file).


[HeroNumberOne.tar.xz]: https://drive.google.com/file/d/1Cxmzm8dk1WzaYS7vfzvzeILS8O78SC92/view?usp=sharing "Serious Sam Classic HeroNumberOne Mod"
[Visual Studio 2015 Community Edition]: https://go.microsoft.com/fwlink/?LinkId=615448&clcid=0x409 "Visual Studio 2015 Community Edition"
[Windows 10 SDK 10.0.14393.795]: https://go.microsoft.com/fwlink/p/?LinkId=838916 "Windows 10 SDK 10.0.14393.795"
[Actions tab]: https://github.com/tx00100xt/SE1-TSE-HNO/actions "Download Artifacts"
