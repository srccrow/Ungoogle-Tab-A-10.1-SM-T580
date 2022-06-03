# Ungoogle Tab A 10.1 SM-T580
Ungoogle Galaxy Tab A 10.1 (2016, SM-T580, Android 12)

# based on

https://gist.github.com/janstuemmel/bebdb5c4e042a0919d0c7cf803f1230c

# Ungoogle Samsung Galaxy Tab A 10.1

Model: SM-T580, Android 7, 64bit

Read first, flash afterwards! File to download are in the Resources section below!

###  Unlock OEM

* Settings > System > About Phone > Build Number (Tap 7 times)
* Enable OEM-Unlock in Developer Options

### Flashing TWRP

* Turn off device and start it in Download-Mode (Power+Home+Volume Down)
* Download Odin (Windows only, use a VM or Heimdall), select TWRP Tar file (AP) and press Start
* After flashing, device will reboot. Quickly press keys for Recovery-Mode (Power+Home+Volume Up)
* You are now in TWRP Recovery

### Installing Rom (and Root)

* Klick Wipe and wipe everything except your external SD card
* Go back and select Install
* Add Zip files
	 * Lineage OS Zip file
	 * [ If you really want Google, add Zip file from opengapps.org ] (Please don't do that :) )
	 * If you want Root add the Magisk Zip file, take v15.3 from above and do not update afterwards (Bootloop!) (required for MicroG and Xposed)
	 * If you want to download Apps from PlayStore anonymously, add YalpStore Zip file (the "contemporary" zip file!)
* Flash the selected Zip files
* Reboot device after flashing, you can now use Lineage OS

### After installing Lineage OS

* Install F-Droid for OpenSource Apps
* Install Xposed Framework Installer from the XDA Developer Thread and install it
* Restart device

### MicroG

* Download Services Core, Services Framework Proxy and FakeStore from microg.org
* Install downloaded APKs
* Add FakeGApps from Xposed for Signature Spoofing
* Add NLP Backends from F-Droid and enable them in MicroG Settings
* If you really want Google Cloud Messaging (GCM, Push Messages), enable Log-In and GCM
* Move GmsCore folder from `/data/app` to `/system/priv-app` (with e.g. ESFileExplorer or adb) (root required)
* Restart your device

### Resources

* [Root Galaxy Tab A 10.1 Youtube Video](https://www.youtube.com/watch?v=1RQNJfpBMs0)
* [Odin Download on droidviews.com](https://www.droidviews.com/download-odin-tool-for-samsung-galaxy-devices-all-versions/)
* [TWRP Download Page for gtaxlwifi on twrp.me](https://dl.twrp.me/gtaxlwifi/)
* [Lineage OS Download on xda-developers.com](https://forum.xda-developers.com/galaxy-tab-a/development/rom-lineageos-14-1-android-7-1-2-nougat-t3706002)
* [Magisk v15.3 Flashable ZIP on github.com](https://github.com/topjohnwu/Magisk/releases/tag/v15.3)
* [YalpStore Download on github.com](https://github.com/yeriomin/YalpStore/releases)
* [Xposed Framework Installer on xda-developer.com (see Thread Attachment)](https://forum.xda-developers.com/showthread.php?t=3034811)
* [MicroG Downloads on microg.org](https://microg.org/download.html)
* [F-Droid](https://f-droid.org/)

---

## Update 2019 (LineageOS 16)

* [XDA Lineage OS 16 (unofficial) SM-T580](https://forum.xda-developers.com/galaxy-tab-a/development/rom-lineageos-15-1-64bit-20180920-t3845016)
* [Magisk v20](https://github.com/topjohnwu/Magisk/releases) works on SM-T580 and Lineage16
* [FDroid Privileged Extension](https://f-droid.org/en/packages/org.fdroid.fdroid.privileged.ota/) for automatic install and update (see zip download down on the page)

### WIP

* [Install MicroG](https://github.com/microg/android_packages_apps_GmsCore/wiki/Installation) in `/system/priv-app` (see note)
* [Signature Spoofing](https://github.com/microg/android_packages_apps_GmsCore/wiki/Signature-Spoofing) for MicroG

#### Alternative

* [Prepare NanoDROID Signature Spoofing for Android 9](https://github.com/Nanolx/NanoDroid/blob/master/doc/DeodexServices.md)
* [Install NanoDROID Patcher](https://github.com/Nanolx/NanoDroid) for MicroG and Signature Spoofing (Steps obove may not be necessary then)
