#buildroot-2017.11

buildroot 2017.11 port of GCW0 opendingux buildroot 2014.05 for RS-97 (JZ4760)

CHANGES
=========

2018.01.11

        Initial commit, buildroot builds properly with initial configuration port of GCW0_defconfig to rs97_defconfig started. Non-applicable packages/libraries/binaries were not removed yet (wifi etc), only dead references from previous version of buildroot. Board files need made, opendingux specifc packages and configs need built.

        -SNESFAN


Instructions
=========
sudo apt-get install sed make binutils build-essential gcc g++ bash patch gzip bzip2 perl tar cpio python unzip rsync file bc wget

git clone git://github.com/SNESFAN/buildroot-2017.git

cd buildroot-2017

make rs97_defconfig

make
