# Ungoogle Tab A 10.1 SM-T580
Ungoogle Galaxy Tab A 10.1 (2016, SM-T580, Android 12)

# Based on

https://gist.github.com/janstuemmel/bebdb5c4e042a0919d0c7cf803f1230c

# Ungoogle Samsung Galaxy Tab A 10.1

Model: SM-T580, Android 12.1, 64bit

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
	 * If you really want Google, add Zip file from https://wiki.lineageos.org/gapps
	 * If you want Root add the Magisk Zip file, https://github.com/topjohnwu/Magisk/releases/tag/v24.1 (required for MicroG and LSPosed)
	 * If you want to download Apps from PlayStore anonymously, add AuroraStore as a standalone package or https://github.com/FriendlyNeighborhoodShane/MinMicroG-abuse-CI
* Flash the selected Zip files
* Reboot device after flashing, you can now use Lineage OS

### After installing Lineage OS

* Install Neo-Store as a standalone package
* Install LSPosed Magisk module from https://github.com/LSPosed/LSPosed
* Restart device

### MicroG

* Use https://github.com/FriendlyNeighborhoodShane/MinMicroG-abuse-CI
* Compile your own version of FakeGapps addressing Android 12 https://github.com/nift4/FakeGApps, consider closed pull-request in order to compile it successfuly inside Android Studio https://github.com/nift4/FakeGApps/pull/1 consider that this version will only work on Android 12.

### Resources

* [TWRP Download Page for gtaxlwifi on twrp.me](https://dl.twrp.me/gtaxlwifi/)
* [Lineage OS Download on xda-developers.com](https://forum.xda-developers.com/galaxy-tab-a/development/rom-lineageos-14-1-android-7-1-2-nougat-t3706002)
* [Magisk v24.1 Flashable ZIP on github.com](https://github.com/topjohnwu/Magisk/releases/tag/v24.1)
* [AuroraStore Download on github.com](https://auroraoss.com/)
* [LSPosed](https://github.com/LSPosed/LSPosed)
* [MicroG](https://github.com/FriendlyNeighborhoodShane)
* [Neo-Store](https://github.com/NeoApplications/Neo-Store)

---

## Update 2022 (LineageOS 19.1)

* [XDA Lineage OS 19.1 (unofficial) SM-T580](https://forum.xda-developers.com/t/lineageos-19-1-for-sm-t580-gtaxlwifi-and-sm-p580-gtanotexlwifi.4432957/page-4#post-86981839)
