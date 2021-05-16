# Changelog

## 1.0.9 (16.05.2021)

- Fixed how OBJ model importing loads files not made with Blender.
- Cleaned up legacy code.
- Fixed ModUpdater glitching out, if the user was not logged in.
- Fixed bunch of issues related to non-premium NexusMods users in mod updating system.
- Fixed cancelling NexusMods login causing it to not work until after game restart.
- Fixed mod updater getting stuck, if mod does not have a default picture set on NexusMods.
- Fixed Credits button linking to the wrong URL.
- Extended logging for some of the features.
- Fixed the top menu label text disappearing too soon.
- Fixed mod auto updates not working for people who have Mods folder outside of MSC

## 1.0.8 (14.05.2021)

- Changed the Keybind setting to allow binding the left and right mousebutton.
- Canceling and deleting keybinds is now done by buttons appearing when binding.
- Deprecated the PartMagnet, BoltMagnet does the exact same thing with no bolts assigned.
- Fixed potential save issue where a different method of calling the SAVEGAME event was used.
- Sorted the mod list after the name of the mods rather than their file names (in case they'd be different from the name).
- Added exception handler for if user exceeds GitHub request limit.
- Added MSCLoader.LoadingScreen.
- Fixed shadow direction on the open settings arrows.	
- ModUpdater class rewritten from scratch - now should be faster and more reliable.
- Added support for ".rar" and ".7z" archive formats, as well as support for "loose" libraries and executables (if they are a part of an archive).
- Improved speed and reliability of update checking system.
- Added "Sources.json" file in ModUpdater folder - enables mods that don't natively support Mod Loader Pro to have auto updates.
- "Sources" file is updated automatically every 2 days.
- Mods not natively supported by Mod Loader Pro (and have been added into Sources.json) will have their info downloaded from NexusMods.
- CoolUpdater: Updated to version 1.0.4.
- CoolUpdater: 403 errors should now be handled correctly.
- CoolUpdater: Switched from Ionic.Zip to SharpCompress.

## 1.0.7 (07.05.2021)

- Bolt components can now operate independently from a BoltMagnet component.
- Added OnScrew event to Bolt component, executed each screw, as well as events OnMaxTightness and OnMinTightness executed when the bolt reach max and min tightness respectively.
- Fixed SettingSlider value text not working properly when the value went into negatives.
- Adjusted UI text and shadows.
- Fixed NexusMods login failing, if user didn't have profile picture set.
- Changed how NexusMods login is being handled, if CoolUpdater couldn't start a web browser
- Removed resources from template, instead adding a guide on the website on how to add resources to your project.
- Addressed an issue related with objects using PartMagnet being not detacheable, if the object has been disabled
- Fixed music not playing after quitting from game to the main menu (issue #5)
- CoolUpdater: Added info page, if CoolUpdater is open by the user
- Uninstaller: Added support for launching the Uninstaller via "Add or remove programs"

## 1.0.6 (02.05.2021)

- Fixed UI scaling on ultrawide resolutions.
- Fixed Nexus out of range exception.
- Fixed user avatar when using Gravatar.

## 1.0.5 (01.05.2021)

- CoolUpdater: Added "Start Game (No Steam)" button.
- Fixed keybinds with None as a modifier.

## 1.0.4 (30.04.2021)

- CoolUpdater: Fixed "Start Game" button not starting the game with Mod Loader Pro.
- Mod Auto Updater should now prioritze archives with .pro.zip extension as intended.

## 1.0.3 (30.04.2021)

- Added "ExecuteCommand" method.
- Fixed update status permanently staying on the main menu, if no mods are installed.
- Fixed compatibility with Cassette mod.

## 1.0.2 (30.04.2021)

- Fixed missing null checks.
- Fixed legacy sliders not updating as they should.

## 1.0.1 (30.04.2021)

- Removed game freezing bug with NexusMods login.

## 1.0 (30.04.2021)

- Initial release.

## 1.0-RC13 (29.04.2021)

- Updated CoolUpdater version to 1.0.
- Fixed hidden settings (SettingString, SettingBoolean, SettingNumber) not loading right away.

## 1.0-RC12 (28.04.2021)

- NexusMods: Mod Loader will now check if Nexus login save data is corrupted.
- Added missing websocket-sharp.dll.
