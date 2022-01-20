# FROST Fast

**Latest Release:**
v1.5.0 (1/20/2022)

- [Preamble](#preamble)
- [Installation](#installation)
  - [Install Microsoft Visual C++ Redistributable Package](#install-microsoft-visual-c-redistributable-package)
  - [Steam Config](#steam-config)
    - [Disable the Steam Overlay](#disable-the-steam-overlay)
    - [Disable the Steam Cloud](#disable-the-steam-cloud)
    - [Change Steam's update behavior](#change-steams-update-behavior)
    - [Set the game language to English](#set-the-game-language-to-english)
  - [Clean Fallout 4](#clean-fallout-4)
  - [Start Fallout 4](#start-fallout-4)
  - [Using Wabbajack](#using-wabbajack)
    - [Download Wabbajack](#download-wabbajack)
    - [Install the modlist](#install-the-modlist)
    - [Errors in Wabbajack](#errors-in-wabbajack)
      - [Wabbajack could not find my game folder](#wabbajack-could-not-find-my-game-folder)
  - [Post-Installation](#post-installation)
    - [Copy Game Folder Files](#copy-game-folder-files)
    - [Edit INI files](#edit-ini-files)
- [Starting FROST for the First Time](#starting-frost-for-the-first-time)
  - [MCM Configuration](#mcm-configuration)
  - [Holotape Configuration](#holotape-configuration)
- [Updating](#updating)
- [Notable Mods](#notable-mods)
- [FAQ](#faq)
- [Removing the Modlist](#removing-the-modlist)
- [Credits and Thanks](#credits-and-thanks)
- [Contact](#contact)
- [Changelog](#changelog)

# Preamble

![FROST Fast Cover](https://github.com/interworlder/FROST-Fast/blob/main/Cover.jpg)

FROST is a total conversion mod which turns Fallout 4 into a challenging survival experience. It has brand new lore, enemies, and gameplay systems.

This modlist, **FROST Fast**, collects multiple mods for you to install with Wabbajack. It's good for anyone who wants to enjoy a modern FROST experience in a relatively fast and easy way--and without being required to learn everything about modding.

Many talented mod authors have contributed to the current state of FROST: which is remarkably bug-free and still being expanded! All credit goes to those authors.

# Installation

These steps will guide you through installing **FROST Fast** for the first time.

If you want to update an existing version of **FROST Fast**, then please jump straight to [Updating](#updating).

## Install Microsoft Visual C++ Redistributable Package

This package is required for Mod Organizer 2. It is likely that you already have this package installed, but if not, go ahead and install it now.

You can download this package directly from [Microsoft](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). Select the x64 version under "Visual Studio 2015, 2017 and 2019". [Here is the direct download link.](https://aka.ms/vs/16/release/vc_redist.x64.exe)

## Steam Config

Right click on _Fallout 4_ in your Steam library and select _Properties_.

### Disable the Steam Overlay

In the _General_ tab, un-tick the checkbox for _Enable the Steam Overlay while in-game_.

(The Steam Overlay can cause issues with ENB, so it is recommended to be turned off. While this modlist does not contain ENB, this setting will help if you choose to add it later.)

### Disable the Steam Cloud

In the same _General_ tab, un-tick the checkbox for _Keep game saves in the Steam Cloud for Fallout 4_.

(Save files generated by the modded game are not compatible with the base game.)

### Change Steam's update behavior

Go to the _Updates_ tab. Under _Automatic Updates_, select the option _Only update this game when I launch it_.

(Updates to Fallout 4 can break existing mods, so we want to make sure Steam does not automatically or unexpectedly update the game.)

### Set the game language to English

Go to the _Language_ tab. Make sure that _English_ is selected.

(This modlist only supports the English language.)

## Clean Fallout 4

If you have modded Fallout 4 in the past, then you must clean your game folder to prevent conflicts. Do not skip this step!

If you have NOT modded Fallout 4 in the past, then you can skip to the [Start Fallout 4](#start-fallout-4) section.

1. Uninstall the game through Steam
2. Delete the game folder, which should be C:\Program Files (x86)\Steam\steamapps\common\Fallout 4 by default
3. Delete the game's save/config folder, which should be C:\Users\yourname\Documents\My Games\Fallout4 by default
4. Reinstall the game through Steam

## Start Fallout 4

You should have a clean installation at this point. Run Fallout 4.

1. Start the game through Steam
2. Click on _Options_ in the game launcher window
3. Set the _Aspect Ratio_ and _Resolution_ to your monitor's native values
4. Set the other graphics settings according to your preferences and hardware
5. Click _OK_ when you are done
6. Click _Play_
7. Wait for the game to load, and then exit when you see the main menu

## Using Wabbajack

### Download Wabbajack

Download the latest release of Wabbajack from [here](https://github.com/wabbajack-tools/wabbajack/releases).

Place the _Wabbajack.exe_ file in a new folder, e.g. C:\Wabbajack.

### Download the modlist

Download the latest release of **FROST Fast** from [Github](https://github.com/interworlder/FROST-Fast/releases). For your convenience, [here is the direct download link](https://github.com/interworlder/FROST-Fast/releases/download/v1.5.0/FROST.Fast.wabbajack). You can save it in the same folder as Wabbajack, e.g. C:\Wabbajack.

### Install the modlist

Keep in mind that downloading and installing the full modlist can take a very long time (depending on your system specs and connection speed).

1. Run Wabbajack.exe
2. Click on _Install From Disk_ and open the file _FROST Fast.wabbajack_
3. Set the _Installation Location_, e.g. C:\FROST-Fast\Install
4. Set the _Download Location_, e.g. C:\FROST-Fast\Download
5. Click the Start button
6. Follow any instructions from Wabbajack (sign into NexusMods, click the download buttons, etc.)
7. Wait for Wabbajack to finish -- this can take a very long time!

### Errors in Wabbajack

If you run into any errors, your first move should be exiting Wabbajack and following the above steps to "Install the modlist" again.

Wabbajack will safely re-check its own installation, pick up where it left off, and re-try any failed downloads.

#### Wabbajack could not find my game folder

Sorry! Wabbajack will not work with pirated versions of the game. If you own a legitimate copy of the game, start over from the beginning of [Installation](#installation) and don't skip any steps.

## Post-Installation

### Copy Game Folder Files

Copy all of the files from "Game Folder Files" in the install location, e.g. C:\FROST-Fast\Install\MO2\Game Folder Files

Paste the files directly into your game folder. In Windows, your game folder defaults to C:\Program Files (x86)\Steam\steamapps\common\Fallout 4

### Edit INI files

Go to your game's save/config folder, which should be C:\Users\yourname\Documents\My Games\Fallout4 by default.

Open Fallout4Prefs.ini and add these lines under \[Display\]:

```
uPipboyTargetHeight=1400
uPipboyTargetWidth=1752
fPipboyScreenEmitIntensityPA=1.25
fPipboyScreenDiffuseIntensityPA=0.15
```

Add this line under \[Imagespace\]:

```
bLensFlare=0
```

Add this line under \[Pipboy\]:

```
bPipboyDisableFX=1
```

Save your changes to Fallout4Prefs.ini.

Next... Open Fallout4.ini, and add this line under \[General\]:

```
sStartingConsoleCommand=cl off
```

Add this line under \[Archive\]:
```
bInvalidateOlderFiles=1
```

And make sure this entry under \[Archive\] is blank, like so:
```
sResourceDataDirsFinal=
```

Save your changes to Fallout4.ini.

## Starting FROST for the First Time

Go to the install location, e.g. C:\FROST-Fast\Install

Run ModOrganizer.exe.

At the top-right, F4SE should be selected already. Click Run.

From the main menu, go to Settings > Gameplay. _New Game Difficulty_ should be set as _Survival_.

This is also a good time to adjust your HUD and Pipboy colors. Go to Settings > Display. I like to use white, so I max out all of these sliders:

* HUD Color R
* HUD Color G
* HUD Color B
* Pip-Boy Color R
* Pip-Boy Color G
* Pip-Boy Color B

Go back to the main menu, and click _New_ to start a new game!

### MCM Configuration

MCM configuration is optional, but feel free to check out all the options available to you.

When you are in-game and finished with character setup, hit _ESC_ and click _Mod Config_.

### Holotape Configuration

There are also a few settings accessible from the in-game Pip-Boy, which come in the form of holotapes.

They might be in your inventory already OR they might need to be crafted at a Chemistry Table.

NPCs Travel is the only one which *must* be configured. Follow the [step-by-step instructions in this image gallery](https://www.nexusmods.com/fallout4/mods/54830/?tab=images).

## Updating

Here are a few things you should know before updating:

* Starting a new game is the safest option after an update. Old save files might be incompatible.
* The Installation Location will be deleted and restored by Wabbajack, so all mods which are not part of this modlist will be removed.
* The Download Location will NOT be deleted by Wabbajack, so you will only download more content if there has been an addition or update.

If you want to know what has changed in the latest version, please review the [Changelog](#changelog).

Otherwise, you can update the modlist by following these steps:

1. Download the latest release of **FROST Fast** from [Github](https://github.com/interworlder/FROST-Fast/releases)
2. Run Wabbajack.exe
3. Click on _Install From Disk_ and open the newest version of the file _FROST Fast.wabbajack_
4. Set the same _Installation Location_, e.g. C:\FROST-Fast\Install
5. Set the same _Download Location_, e.g. C:\FROST-Fast\Download
6. Check the box _Overwrite Installation_
7. Click the Start button
8. Follow any instructions from Wabbajack (sign into NexusMods, click the download buttons, etc.)
9. Wait for Wabbajack to finish

## Notable Mods

<details>
  <summary>Click to expand!</summary>

**Fallout 4 Script Extender (F4SE)**

**Buffout 4**

**Unofficial Fallout 4 Patch**

**Mod Configuration Menu**

**FO4 Photo Mode**

**Raw Input - The Ultimate Mouse Sensitivity Fix**

**High FPS Physics Fix**

**Binaural 3D Surround Sound for Headphones - HRTF**

**Vats over there - Increased V.A.T.S Distance**

**LevelUpMenuEx**

**Extended Dialogue Interface**

**Silent UI**

Disables quest and XP-related sound effects. Disables faction music. Disables perk activation sounds. Disables battle music and player death music.

**DEF_UI Iconlibs Rescaled and Fixed - Colored**

**FallUI**

**FallUI - HUD**

**FallUI - Workbench**

**FallUI - Confirm Boxes**

**FallUI - Map**

**Ultra Interior Lighting**

**Ultra Exterior Lighting**

**Project Reality Footsteps (Snow Edition)**

**Scavver's Toolbox**

**Campsite - Simple Wasteland Camping**

Allows the player to sleep and save anywhere (if they are willing to craft and carry a sleeping bag).

**Far Harbor Trap Overhaul**

**Grab and Eat All-in-One**

**NPCs Travel**

**Remove Low Health Blur**

Removes the blur applied when the player's health is low, but keeps the blur when the player's head is crippled.

**Death effects Removed**

Removes the intense blur applied upon death.

**Real Time Death (No Slow mo) - 20 seconds**

Gives the player a sad (or hilarious) moment to reflect on their most recent death.

**Smokeable Cigars - Cigarettes - Joints - With HardCore Auto Save**

Allows the player to save anywhere (if they are willing to use an addictive drug).

**Less Cigarette and Cigar Loot**

**Fill'em Up Again (Dynamic Bottle Recyclation)**

**LooksMenu**

Improves the character creation interface.

**FROST Survival Simulator**

**Alternative Farming for FROST**

**FROST Unofficial Updates**

**FROST - Nuka World AddOn**

**Freeze Intimidation Overhaul**

**FROST Survival Kit**

**FROST Downtown Linked Workbenches**

**Frost Downtown Monohome**

Adds a player home to Downtown. If the radio is too much, open the console, select it, and use the "disable" command.

**Frost Plus**

**FROST - More Starting Locations**

**FROST - It Snowed - Winter Textures**

**FROST - Snowy Weathers**

**Frost - Dogmeat resurrected**

Adds the option of recruiting a canine companion. Makes FROST easier because the dog cannot be killed, alerts on nearby enemies, and adds sanity... but it is optional. 

**See-Through-Scopes**

**FROST - Exterior Cell Fixes**

**FROST - Interior Cell Fixes**

**Ruddy88's Simple Sorter**

This ESP is not required and therefore disabled, but I am including it just in case someone wants to generate their own item sorting list using Complex Sorter.

**FROST Fast - Complex Sorter List**

This is a Complex Sorter list generated specifically for the FROST Fast modlist.

**Satellite World Map**

**Far Harbor Satellite Map**

**Nuka-World Satellite Map**

</details>

## FAQ

**Why do enemies and mines sometimes disappear after loading a save?**

This is a bug from vanilla Fallout 4 which was unfortunately never fixed by Bethesda. You can get past it by quitting the game to desktop, starting the game again, and loading the save. This will ensure that enemies and explosives are respawned correctly.

**Can I add player textures, 3d model replacers, and other cosmetic mods?**

Yes, you would want to put those mods under the "Player Appearance" separator in Mod Organizer 2. Remember to re-order your plugins (on the right) so they match the mod list (on the left).

**Why is the R88 Simple Sorter mod included in the modlist?**

This ESP is not technically required, but I have included it just in case someone wants to generate their own custom item sorting list using Complex Sorter.

**Can I add NSFW (Not Safe For Work) mods?**

Yes, you can, but unfortunately I cannot provide support in that area!

**Why isn't the PANPC mod included in the modlist?**

The current download license for Pack Attack NPC forbids its inclusion from any modpack or automated modlist. Sorry! Of course, feel free to add the mod yourself (along with its FROST compatibility patch).

## Removing the Modlist

In order to uninstall **FROST Fast** completely, you will need to delete your Installation and Download Locations. If you followed this guide verbatim, then you should delete C:\FROST-Fast entirely.

Next, follow all of the steps in the [Clean Fallout 4](#clean-fallout-4) section again. Done! You should have a clean installation of Fallout 4 again.

(Optional) If you do not want Wabbajack anymore, you will need to delete your Wabbajack folder too. If you followed this guide verbatim, then you should delete C:\Wabbajack.

(Optional) And if you do not want Fallout 4 anymore, then you should remove Fallout 4 through Steam.

## Credits and Thanks

All credit and thanks go to the Fallout 4 modding community and the Wabbajack development community. And thanks to you for reading this!

## Contact

Bug reports and feature requests should go into the [Github issues tracker](https://github.com/interworlder/FROST-Fast/issues) for **FROST Fast**.

## Changelog

**v1.5.0**

* Added Game Configuration Menu
* Added Sprint Stuttering Fix
* Added Valius High Resolution Texture Pack 4K
* Added Natural Landscapes 4K
* Added FlaconOil's Complete Retexture Project
* Added Enhanced Blood Textures
* Added Puddle Remover Plus
* Added Magnetic Coils and Capacitors - A Gauss Rifle Retexture
* Added Wasteland Illumination Shadow Version (again)
* Added Animated Chems Redone
* Added GNN National Broadcast - Diamond City Radio without Travis 2.0.0 Update
* Added Spitfire Enhanced Muzzle FX
* Added Wattz Laser Gun
* Added Fallout 3 10mm SMG
* Added Fire Axe
* Added Murdering Chainsaw
* Added AK74M
* Added Vivid Weathers

**v1.4.1**

* **IMPORTANT:** If you are updating FROST Fast to this version, follow the steps in [Updating](#updating) and then follow the steps in [Copy Game Folder Files](#copy-game-folder-files) as well.
* Edited the install process for F4SE Scripts, Address Library, and Buffout 4 to use MO2's virtualized mod folders
* Added Binaural 3D Surround Sound for Headphones - HRTF to the Game Folder Files again (they were missing from the previous version v1.4.1)

**v1.4.0**

* **IMPORTANT:** If you are updating FROST Fast to this version, follow the steps in [Updating](#updating) and then follow the steps in [Copy Game Folder Files](#copy-game-folder-files) as well.
* Fixed file structure and missing files in the Game Folder Files for F4SE and Buffout4
* Fixed config of See-Through-Scopes to include patches for custom weapons like the Service Rifle
* Added Ultra Exterior Lighting
* Added FROST - Exterior Cell Fixes and FPS Boost
* Added FROST - Exterior Cell Fixes -- Nuka World Patch
* Added FROST - Exterior Cell Fixes -- Ultra Exterior Lighting Patch
* Added Fill'em Up Again (Dynamic Bottle Recyclation)
* Added Disable Enemy Killmove component of Realistic melee range and killmove (Frost supported)
* Added Binaural 3D Surround Sound for Headphones - HRTF to the Game Folder Files
* Added FROST - Accuracy Reversion
* Removed Wasteland Illumination Shadow Version
* Removed FROST - Nuka World AddOn - Performance Patch
* Removed FROST - Vanilla Signs Removal

**v1.3.3**

* Added Winter Commonwealth Pines
* Added FROST - Vanilla Signs Removal
* Added FROST - Headless Dead Ferals Fix
* Added FROST - Hunkered Down - Settlements

**v1.3.2**

* Added FROST - Accessible Fort Strong
* Removed Immersive HUD - iHUD
* Updated FROST Fast Complex Sorter List to use latest version v1.3.2

**v1.3.1**

* Updated Mod Organizer 2 to use latest version v2.4.2
* Wabbajack should now point to the correct download location for Mod Organizer 2: Github instead of Nexus

**v1.3.0**

* Updated FROST Unofficial Updates to use latest version v0.9
* Updated FROST - Nuka World AddOn to use latest version v1.3
* Added FROST NPCs Travel compatibility patch

**v1.2.1**

* Removed Unequip Pipboy
* Removed Pipboy Flashlight and its compatibility patch for Unequip Pipboy

**v1.2.0**

* Updated FROST Plus to use latest version v0.4.7
* Updated FROST Interior Cell Fixes to use latest version v2.0
* Added Pip-Boy Flashlight with a compatibility patch for Unequip Pipboy
* Added FROST - Accessible Med-Tek Research
* Removed Atomic Radio to reduce download size
* Removed More Where That Came From - Diamond City Radio Edition to reduce download size
* Removed VHF Repeater Realistic Ham Radio to reduce download size

**v1.1.0**

* Added Silent UI to disable intrusive sound effects and music.
* Added Immersive HUD - iHUD to allow hiding of HUD elements using context-sensitive logic.
* Reconfigured Project Reality Footsteps so it is using the FROST-appropriate 1.6 Snow Edition.
* Removed Barefoot Footstep Extended because its low bitrate samples can be grating for players with headphones.
* Other notes: The readme now shows Notable Mods instead of a full list of Included Mods for ease of documentation. The list will be shortened further over time.

**v1.0.0**

* This is the first public release!
