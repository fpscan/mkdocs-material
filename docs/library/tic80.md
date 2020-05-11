# TIC-80

## Background

[TIC-80](https://tic.computer) is a fantasy computer for making, playing and sharing tiny games.

The TIC-80 core has been authored by

- Rob Loach

The TIC-80 core is licensed under

- [MIT](https://github.com/nesbox/TIC-80/blob/master/LICENSE)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Requirements

None

## BIOS

The TIC-80 core does not feature BIOS use.

## Extensions

Content that can be loaded by the TIC-80 core have the following file extensions:

- `.tic` (TIC-80 cart)

RetroArch database(s) that are associated with the TIC-80 core:

- [`TIC-80.rdb`](https://github.com/libretro/libretro-database/blob/master/rdb/TIC-80.rdb)

## Features

Frontend-level settings or features that the Theodore core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Saves             | ✔         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | [✔](https://tic.computer/play?cart=893)         |
| Core Options      | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | [✔](https://github.com/libretro/libretro-database/tree/master/cht/TIC-80)         |
| Controls          | ✔         |
| Remapping         | ✕         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The TIC-80 core's internal core name is `tic80`.

### Geometry and timing

- The TIC-80 core's base width is 240 pixels.
- The TIC-80 core's base height is 136 pixels.

## Usage

1. Download a [TIC-80 cart](https://tic.computer/play)
    - Example: [TIC-80 Mario Bros?](https://tic.computer/play?cart=223)

2. Launch the cart through the TIC-80 core

## Core options

The TIC-80 core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Mouse API instead of Pointer** [tic80_mouse] (**disabled**|enabled)
- **Mouse Cursor** [tic80_mouse_cursor] (**disabled**|dot|cross|arrow)

## Controllers

The TIC-80 core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 - 4 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad - Stay on this.
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad

!!! attention
	What the buttons do are game specific.

| User 1 - 4 Remap descriptors | RetroPad Inputs                                |
|------------------------------|------------------------------------------------|
| A                            | ![](/image/retropad/retro_b.png)             |
| X                            | ![](/image/retropad/retro_y.png)             |
| Select                       | ![](/image/retropad/retro_select.png)        |
| D-Pad Down                   | ![](/image/retropad/retro_dpad_down.png)     |
| D-Pad Left                   | ![](/image/retropad/retro_dpad_left.png)     |
| D-Pad Right                  | ![](/image/retropad/retro_dpad_right.png)    |
| B                            | ![](/image/retropad/retro_a.png)             |
| Y                            | ![](/image/retropad/retro_x.png)             |
| L                            | ![](/image/retropad/retro_l1.png)            |
| R                            | ![](/image/retropad/retro_r1.png)            |

## External Links

- [TIC-80 Github Repository](https://github.com/nesbox/TIC-80/)
- [Report Libretro TIC-80 Core Issues Here](https://github.com/nesbox/TIC-80/issues)
- [Libretro TIC-80 Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/tic80_libretro.info)
- [Libretro TIC-80 Database](https://github.com/libretro/libretro-database/blob/master/rdb/TIC-80.rdb)
- [Libretro TIC-80 Thumbnails](https://github.com/libretro-thumbnails/TIC-80)
- [Libretro TIC-80 Cheats](https://github.com/libretro/libretro-database/tree/master/cht/TIC-80)
