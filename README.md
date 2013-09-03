INITIALIZING REPOSITORY
=======================

Init core trees without any device/kernel/vendor :

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2

Init repo with all devices, kernels and vendors supported by OurROM :

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,kernel,device,vendor

Init repo only for a particular device

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,<devicename>,<vendorname>

for example, to init only trees needed to build mako

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,mako,lge

sync repo

    $ repo sync -j16
