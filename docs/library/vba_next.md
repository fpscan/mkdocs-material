# Nintendo - Game Boy Advance (VBA Next)

## Background

VBA Next is a Game Boy Advance emulator based on VBA-M 2011 with backported patches for performance and compatibility improvements.

### Author/License

The VBA Next core has been authored by

- Forgotten
- VBA-M Team
- Squarepusher

The VBA Next core is licensed under

- [GPLv2](https://github.com/libretro/vba-next/blob/master/LICENSE)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Extensions

Content that can be loaded by the VBA Next core have the following file extensions:

- .gba

## Databases

RetroArch database(s) that are associated with the VBA Next core:

- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## BIOS

Required or optional firmware files go in the frontend's system directory.

!!! warning
	In order for the Game Boy Advance BIOS to be used, the 'Use bios if available' core option must be set to On.

|   Filename    |    Description                    |              md5sum              |
|:-------------:|:---------------------------------:|:--------------------------------:|
| gba_bios.bin  | Game Boy Advance Image - Optional | a860e8c0b6d573d191e4ec7db1b1e4f6 |

## Features

Frontend-level settings or features that the VBA Next core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✕         |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The VBA Next core's directory name is 'VBA Next'

The VBA Next core saves/loads to/from these directories.

**Frontend's Save directory**

- 'content-name'.srm (Cartridge battery save)

**Frontend's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The VBA Next core's core provided FPS is 59.727
- The VBA Next core's core provided sample rate is 32000 Hz
- The VBA Next core's core provided aspect ratio is 3/2

## Core options

The VBA Next core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Use bios if available (Restart)** [vbanext_bios] (Off/**On**)

	Uses BIOS present in RetroArch's system directory. Look at the [BIOS section](https://docs.libretro.com/library/vba_next/#bios) for more information.
	
??? note "Use bios if available - On"
	![](/image/core/vba_nextbios.png)

## Controllers

The VBA Next core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- None - Doesn't disable input
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad

![](/image/controller/gba.png)

| User 1 Remap descriptors | RetroPad Inputs                           |
|--------------------------|-------------------------------------------|
| B                        | ![](/image/retropad/retro_b.png)    |
| Select                   | ![](/image/retropad/retro_select.png)     |
| Start                    | ![](/image/retropad/retro_start.png)      |
| D-Pad Up                 | ![](/image/retropad/retro_dpad_up.png)    |
| D-Pad Down               | ![](/image/retropad/retro_dpad_down.png)  |
| D-Pad Left               | ![](/image/retropad/retro_dpad_left.png)  |
| D-Pad Right              | ![](/image/retropad/retro_dpad_right.png) |
| A                        | ![](/image/retropad/retro_a.png)    |
| L                        | ![](/image/retropad/retro_l1.png)    |
| R                        | ![](/image/retropad/retro_r1.png)         |

## Compatibility

| Game                                              | Issue                                                                                              |
|---------------------------------------------------|----------------------------------------------------------------------------------------------------|
| Boktai Trilogy 	                                | The solar sensor is not emulated.                                                                  | 
| Croket! 2 – Yami no Bank to Banqueen              | Heavy slowdown when approaching the snowman in the beginning.                                      |
| Digimon Racing (Europe) 	                        | Freezes during the intro. This can be avoided by enabling linking in the standalone VBA-M release. |
| Drome Racers 	                                    | Only shows a black screen after the THQ logo.                                                      |
| Hamtaro: Ham-Ham Games 	                        | Locks up if the opening cinematics aren’t skipped.                                                 |
| Hot Wheels - Stunt Track Challenge                | Resets itself when trying to go in-game.                                                           |
| Jurassic Park III: Park Builder 	                | Unreadable glitched text.                                                                          |
| Koro Koro Puzzle Happy Panechu! 	                | The tilt sensor is not emulated.                                                                   |
| Moto GP 	                                        | Black screen, loud screeching noise.                                                               |
| Phantasy Star Collection 	                        | Digital Eclipse logo sound effect is missing. Phantasy Star 1 flickers.                            |
| SSX 3 	                                        | Graphics glitches. Seems pitch-related. (1)                                                        |
| Super Mario Advance 2: Super Mario World (Europe) | The program crashes during the final fight, when Bowser approaches (zoom mode 7)                   |
| WarioWare: Twisted!                               | The tilt sensor is not emulated.                                                                   |
| Yoshi’s Universal Gravitation                     | The tilt sensor is not emulated.                                                                   |

??? note "1"
	![](/image/core/vba_next/ssx.png)

## External Links

- [Libretro VBA Next Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/vba_next_libretro.info)
- [Libretro VBA Next Github Repository](https://github.com/libretro/vba-next)
- [Report Libretro VBA Next Core Issues Here](https://github.com/libretro/vba-next/issues)

### See also

#### Nintendo - Game Boy Advance

- [Nintendo - Game Boy Advance (Beetle GBA)](https://docs.libretro.com/library/beetle_gba/)
- [Nintendo - Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Nintendo - Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Nintendo - Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [Nintendo - Game Boy Advance (TempGBA)](https://docs.libretro.com/library/tempgba/)
- [Nintendo - Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vba_m/)
