CyanogenMod 11.0 device configuration for LG L70 Dual 

How to build:
-------------

Initializing a Build Environment:

    https://source.android.com/source/initializing.html

Initialize repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-11.0

    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/vm03/android_local_manifest/master/local_manifest.xml
    repo sync
    vendor/cm/get-prebuilts

Compile:

    . build/envsetup.sh
    brunch cm_w5ds-userdebug
