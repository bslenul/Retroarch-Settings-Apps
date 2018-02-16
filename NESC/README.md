# Retroarch-Settings-Apps

![Retroarch-Settings-Apps](https://i.imgur.com/msXRJqZ.png "Retroarch-Settings-Apps")

## Different versions

   - KMFD_users_BEFORE_2-15-18_update: if you're using a version of KMFDManic core set BEFORE his 2-15-18 update.
   - KMFD_users_AFTER_2-15-18_update: if you're using 2-15-18 version of KMFDManic core set or later.
   - retroarch-clover_users: if you're using Cluster's retroarch-clover core set.

# What these apps do:

## DefaultSettingsAll.zip / RetroArch - Default settings (All)

   - Will replace current `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` with default ones.
   - Will delete the content of `/etc/libretro/.config/retroarch/config` folder (game and core overrides + remap files).

## DefaultSettingsKeepOverrides.zip / RetroArch - Default settings (keep overrides)

   - Will only replace current `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` with default ones.
   - Game and core overrides + remap files are untouched.

## DeleteOverrides.zip / RetroArch - Delete game and core overrides

   - Will only delete game and core overrides.
   - Retroarch settings and remap files are untouched.

## DeleteRemaps.zip / RetroArch - Delete remap files

   - Will only delete remap files.
   - Retroarch settings, game and core overrides are untouched.

## MakeBackup_NAND.zip / RetroArch - Make settings backup

   - Will copy `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/ra_backup`.
   - Will copy `/etc/libretro/.config/retroarch/config` folder in `/etc/ra_backup`.

## RestoreBackup_NAND.zip / RetroArch - Restore settings backup

   - Will restore `/etc/ra_backup/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/libretro`.
   - Will restore `/etc/ra_backup/config` folder in `/etc/libretro/.config/retroarch`.

## DeleteBackup_NAND.zip / RetroArch - Delete backup folder

   - Will delete `/etc/ra_backup` folder from the NAND.

## MakeBackup_USB.zip / RetroArch - Make settings backup

   - Will copy `/etc/libretro/retroarch.cfg` and `retroarch-core-options.cfg` in `/media/data/ra_backup` (= `usb:\data\ra_backup`).
   - Will copy `/etc/libretro/.config/retroarch/config` folder in `/media/data/ra_backup`.

## RestoreBackup_USB.zip / RetroArch - Restore backup

   - Will restore `/media/data/ra_backup/retroarch.cfg` and `retroarch-core-options.cfg` in `/etc/libretro`.
   - Will restore `/media/data/ra_backup/config` folder in `/etc/libretro/.config/retroarch`.
