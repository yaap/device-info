# For first-timers:
- Download ROM zip and recovery zip.
- Boot to bootloader.
- Run __fastboot update --skip-reboot recovery-YAAP-*.zip__
- Follow Firmware flashing steps.
- Run __fastboot reboot recovery__
- Format data with the recovery.
- Click apply for update.
- Run __adb sideload YAAP*.zip__
- Reboot to system.
# For first-timers(SD card):
- Download ROM zip and recovery zip.
- Copy ROM zip to SD card.
- Boot to bootloader.
- Run __fastboot update --skip-reboot recovery-YAAP-*.zip__
- Follow Firmware flashing steps.
- Run __fastboot reboot recovery__
- Format data with the recovery.
- Click apply update with SD card.
- Choose the ROM zip and click the power button to confirm.
- Reboot to system once it is flashed.
# For dirty-flashers:
- Download ROM zip.
- Follow Firmware flashing steps if fw is updated.
- Boot to recovery.
- Click apply for update.
- Run __adb sideload YAAP*.zip__
- Reboot to system.
# For OTA-flashers:
- Follow Firmware flashing steps if fw is updated.
- Boot back to system.
- Go to Settings->System->YAAP Updater.
- Click Download.
- Be very patient after this step as __*OTA is a slow process and will take approximately 30-45 minutes*__ (It would specifically be stuck at 68% for that amount of time alone!).
- Reboot after it is done.
# Firmware flashing steps:
- Download recommended fw.
- Boot to bootloader.
- Run __fastboot update --skip-reboot sunny-fw.zip__
