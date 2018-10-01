<p align="center">
    <img src="https://img.xda-cdn.com/7o7Id5HtrJgXhi02dSc38NpUZr0=/https%3A%2F%2Fi.imgur.com%2FMy52Bu0.png" />
</p>

Simplix Blue
============

Get started
-----------

Before trying to build the ROM yourself, make sure you have established your building environment.

For more info on how to do exactly that, check [AOSP's official documentation](https://source.android.com/setup/build/initializing).

Downloading the source
----------------------

You can download the source by simply doing:

    repo init -u https://github.com/SimplixDot/platform_manifest.git -b pie
    repo sync --no-tags --no-clone-bundle --force-sync -c
    
On multithread CPUs (which you probably have, considering you would like to build Android :P) you can set multiple sync jobs by doing:

    repo sync --no-tags --no-clone-bundle --force-sync -c -jX

where X is the count of your CPU threads.

Building the ROM
----------------

CosmicOS (on which our ROM is based) comes with a handy script for building the system. You can use it just by typing this from your work folder:

    . build-simplix.sh <your device codename>
    
or you can manually build by doing:

    . build/envsetup.sh
    lunch simplix_<your device codename>-userdebug
    brunch <device>
    
Credits
-------
 * [**Cosmic OS**](https://github.com/Cosmic-OS)
 * [**Lineage OS**](https://github.com/LineageOS)
 * [**Pixel Experience**](https://github.com/PixelExperience)
 
 
