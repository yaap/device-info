# Keep in mind...
- System is Read-Only (restricts making changes to overlays, system APKs, etc.)
- DO NOT USE any other recovery than YAAP recovery which is included.
- Use the RESPECTIVE recovery for RESPECTIVE builds. (e.g if you want to flash vanilla build, use vanilla recovery, if you want to flash gapps build, flash gapps recovery)
- You MUST format data with given YAAP recovery.
- YOU MUST CLEAN FLASH if you are coming from any other ROM or stock.
- Formatting with YAAP Recovery (yes, I mean YAAP Recovery ONLY) is MUST during clean flash.
- First boot WILL take 5-10 minutes, DO NOT PANIC! (only applicable to 20241009 build)
- Required Firmware: Android 14 U1TD34M.94-12-7 or newer. Do not flash on Android 15 firmware.
- Any slot must not be empty, meaning if you have ever used blankflash or flashed stock ROM using RSA or got a new phone, then make sure you got any ota, otherwise don't flash!
- Do NOT try to flash gapps on vanilla build, it WILL NOT work!
- Do NOT try to flash anything other than the ROM in recovery, it WILL NOT work!
- SD card flashing only supports vFAT(FAT12, FAT16, FAT32) and exFAT filesystems.

# For first-timers:
- Download ROM zip and vendor_boot.img.
- Boot to bootloader.
- Run __fastboot reboot fastboot__
- Run __fastboot flash vendor\_boot vendor\_boot.img__
- Run __fastboot reboot bootloader__
- Run __fastboot reboot recovery__
- Format data with the recovery.
- Click apply for update.
- Run __adb sideload YAAP*.zip__
- Reboot to system.
# For first-timers(SD card):
- Download ROM zip and vendor_boot.img.
- Copy ROM zip to SD card.
- Boot to bootloader.
- Run __fastboot reboot fastboot__
- Run __fastboot flash vendor\_boot vendor\_boot.img__
- Run __fastboot reboot bootloader__
- Run __fastboot reboot recovery__
- Format data with the recovery.
- Click apply update with SD card.
- Choose the ROM zip and click the power button to confirm.
- Reboot to system once it is flashed.
# For dirty-flashers:
- Download ROM zip.
- Boot to recovery.
- Click apply for update.
- Run __adb sideload YAAP*.zip__
- Reboot to system.
# For OTA-flashers:
- Boot back to system.
- Go to Settings->System->YAAP Updater.
- Click Download.
- Be very patient after this step as __*OTA is a slow process and will take approximately 30-45 minutes*__ (It would specifically be stuck at 68% for that amount of time alone!).
- Reboot after it is done.
