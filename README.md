The Android Open Source Project Nougat
===========

To initialize your local repository using the AOSP-G3 trees & MikaalSky vs985 files, use a command like this:
````bash
repo init -u git://github.com/MikaalSky/manifest.git -b nougat
```
Then to sync up:
````bash
repo sync -c -f -j8 --force-sync --no-clone-bundle --no-tags
```
Finally to build (hopefully):
````bash
. build/envsetup.sh && lunch aosp_vs985-userdebug && make bacon -j8
```
