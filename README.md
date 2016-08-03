# angler-cm-proprietary
scripts and tool for extracting proprietary blobs from angler factory image

extract-files-from-nexus-image.sh is modified from 
https://raw.githubusercontent.com/CyanogenMod/android_device_huawei_angler/0e35b7973dc899155a6b045f4d0b0f42d17ef954/extract-files-from-nexus-image.sh

usage:

1. `git clone https://github.com/SBUNetSys/smali.git` and `git clone https://github.com/SBUNetSys/android-simg2img.git`

2. in smali dir, type `./gradlew build`; 
in android-simg2img, type `make` and  `ln -s ${PWD}/simg2img ~/bin/simg2img` (I assume ~/bin is in the PATH)

3. put extract-files-from-nexus-image.sh in device/huawei/angler/ dir, and execute it.

4. execute device/huawei/angler//extract-files.sh "/tmp/extract-files/angler/mtc20f"  "your smali folder"
