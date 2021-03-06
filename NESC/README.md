# Retroarch-Settings-Apps

![Retroarch-Settings-Apps](https://i.imgur.com/msXRJqZ.png "Retroarch-Settings-Apps")

# What these apps do:

## DefaultSettingsAll.zip / RetroArch - Default settings (All)

   - Will replace current `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` with default ones.
   - Will delete the content of `/etc/libretro/.config/retroarch/config` folder (game and core overrides + remap files).
   - Will restore the optional N64 remap files from KMFDManic to `/etc/libretro/.config/retroarch/config/remaps`.
   
### IMPORTANT

   - Default files are for retroarch-clover 1.1c, if you're using another version of retroarch you need to replace these files.
   - For example if you're using `_km_retroarch_171_standard_2_23_18` open the .hmod with 7zip, winrar or whatever, you'll see a file with no extension:
   ![Opening .hmod](https://i.imgur.com/qbwUdcF.png "Opening .hmod")
   - Open this file by double-clicking it, now go to `\etc\libretro`, you should the 2 .cfg files that we need:
   ![.cfg files inside the .hmod](https://i.imgur.com/nktevXz.png ".cfg files inside the .hmod")
   - Go to `\hakchi2\games\CLV-P-ALLRA`, drag the 2 .cfg files from the .hmod and overwrite the ones already there.

## DefaultSettingsKeepOverrides.zip / RetroArch - Default settings (keep overrides)

   - Will only replace current `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` with default ones.
   - Game and core overrides + remap files are untouched.
   - See the "**IMPORTANT**" section above, but overwrite the files in `\hakchi2\games\CLV-P-RASET` instead.

## DeleteOverrides.zip / RetroArch - Delete game and core overrides

   - Will only delete game and core overrides.
   - Retroarch settings and remap files are untouched.

## DeleteRemaps.zip / RetroArch - Delete remap files

   - Will only delete remap files.
   - Retroarch settings, game and core overrides are untouched.

# /!\ Backup and restore settings /!\

   - Add only one MakeBackup zip in Hakchi2: `MakeBackup_NAND` **OR** `MakeBackup_USB` **OR** `MakeBackupAdvanced_USB`.
   - Same for RestoreBackup: `RestoreBackup_NAND` **OR** `RestoreBackup_USB` **OR** `RestoreBackupAdvanced_USB`.
   - The RestoreBackupAdvanced_USB will copy the entire `/etc/libretro/.config` folder (useful if you have RetroArch overlays and/or cheats) + `/etc/libretro/system` (your BIOS folder).
   - Depending on the number and size of BIOS/cheats/overlays, it can take some time to backup/restore.

## MakeBackup_NAND.zip / RetroArch - Make settings backup

   - Will copy `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/ra_backup`.
   - Will copy `/etc/libretro/.config/retroarch/config` folder in `/etc/ra_backup`.

## RestoreBackup_NAND.zip / RetroArch - Restore settings backup

   - Will restore `/etc/ra_backup/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/libretro`.
   - Will restore `/etc/ra_backup/config` folder in `/etc/libretro/.config/retroarch`.

## MakeBackup_USB.zip / RetroArch - Make settings backup

   - Will copy `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` in `/media/data/ra_backup` (= `usb:\data\ra_backup`).
   - Will copy `/etc/libretro/.config/retroarch/config` folder in `/media/data/ra_backup`.

## RestoreBackup_USB.zip / RetroArch - Restore backup

   - Will restore `/media/data/ra_backup/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/libretro`.
   - Will restore `/media/data/ra_backup/config` folder in `/etc/libretro/.config/retroarch`.

## MakeBackupAdvanced_USB.zip / RetroArch - Make settings backup

   - Will copy `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/ra_backup`.
   - Will copy `/etc/libretro/.config` folder in `/media/data/ra_backup`.
   - Will copy `/etc/libretro/system` folder in `/media/data/ra_backup`.
   
## RestoreBackupAdvanced_USB.zip / RetroArch - Restore backup

   - Will restore `/media/data/ra_backup/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/libretro`.
   - Will restore `/media/data/ra_backup/.config` folder in `/etc/libretro`.
   - Will restore `/media/data/ra_backup/system` folder in `/etc/libretro`.

## DeleteBackup.zip / RetroArch - Delete backup folder

   - Will delete `/etc/ra_backup` folder from the NAND.
   - Will delete `/media/data/ra_backup` folder from the USB drive.
