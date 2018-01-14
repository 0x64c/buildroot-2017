# buildroot-2017.11

buildroot 2017.11 port of GCW0 opendingux buildroot 2014.05 for RS-97 (JZ4760)

## [Unreleased]

## Changelog

## 2018.01.13
### Added 
- file structure from gcw0 buildroot

### Changed
- fixed dependencies in file skeleton (/var/tmp, etc/shawdow)
- gmenu2x support for RS97(640x480)

## 2018.01.12
### Added
- Dingux Commander
- Gmenu2x
- ipkg
- libxdgmime
- pwswd

### Changed 
- config menu under packages>opendingux to reflect opendingux additions to buildroot
- removed warning about ipkg in legacy config options
        
## 2018.01.11
### Added
- Initial commit

## Todo
- add support for rs97 in pwswd (hotkey configs)
- fix bennugd
- fix etna_viv (if needed)
- remove connectivity options as default (only need ip over usb)

## Instructions

sudo apt-get install sed make binutils build-essential gcc g++ bash patch gzip bzip2 perl tar cpio python unzip rsync file bc wget

git clone git://github.com/SNESFAN/buildroot-2017.git

cd buildroot-2017

make rs97_defconfig

make
