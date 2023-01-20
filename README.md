# blendOS ISO build scripts
The blendOS build scripts are used to build the blendOS installation ISO images.

## Building the ISO
### 1. Install the build tools
```
sudo pacman -S archiso
```
### 2. Pull the repository
```
git clone https://github.com/blend-os/blendiso.git
```
### 3. Build
```
cd blendiso
sudo mkarchiso -v -w workdir/ -o out/ .
```
Once the building process is finished you can find the ISO image in the `./out` directory.
### 4. Rebuilding the ISO
When building a second time you will have to remove the `./out` and `./workdir` directories.
```
sudo rm -rf ./out ./workdir
```

## Credits
This is based on Arkane Linux's ISO build scripts.

## Development
Contributions, in any form, be it code or ideas are always welcome!
### Getting started as a contributor
Refer to the ArchWiki page on [Archiso](https://wiki.archlinux.org/title/Archiso) for information. Or follow the introductionary videos and articles by Erik Dubois on the Carli project, if you are GNU/Linux savvy the [Carli-1](https://www.arcolinuxiso.com/carli-1/) series of videos should provide you with all the information you need to get started.
