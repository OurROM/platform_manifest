INITIALIZING REPOSITORY
=======================

Init core trees without any device/kernel/vendor :

<<<<<<< HEAD
    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2
=======
    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat
>>>>>>> 3acfc8533c7a20e2073ed0ea3ed2638d56800862

Init repo with all devices, kernels and vendors supported by OurROM :

<<<<<<< HEAD
    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,kernel,device,vendor

Init repo only for a particular device :

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,<devicename>,<vendorname>
=======
    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat -g all,kernel,device,vendor

Init repo only for a particular device :

    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat -g all,-notdefault,<devicename>,<vendorname>
>>>>>>> 3acfc8533c7a20e2073ed0ea3ed2638d56800862

for example, to init only trees needed to build mako

<<<<<<< HEAD
    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,mako,lge
=======
    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat -g all,-notdefault,mako,lge
>>>>>>> 3acfc8533c7a20e2073ed0ea3ed2638d56800862

Init repo for multiple devices

<<<<<<< HEAD
    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,<devicename1>,<devicename2>,<devicename3>,<vendorname1>,<vendorname2>,<vendorname3>

for example, to init trees needed to build mako and grouper
=======
    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat -g all,-notdefault,<devicename1>,<devicename2>,<devicename3>,<vendorname1>,<vendorname2>,<vendorname3>

for example, to init trees needed to build mako and flo :

    $ repo init -u https://github.com/AOKP/platform_manifest.git -b kitkat -g all,-notdefault,mako,flo,lge,asus
>>>>>>> 3acfc8533c7a20e2073ed0ea3ed2638d56800862

    $ repo init -u https://github.com/OurROM/platform_manifest.git -b jb-mr2 -g all,-notdefault,mako,grouper,lge,asus

sync repo :

    $ repo sync
