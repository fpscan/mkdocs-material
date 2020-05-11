# RetroArch input and joypad drivers

RetroArch makes use of two input systems in order to support the full range of input devices available across RetroArch's supported platforms.

- **Input Drivers** provide access to keyboards, mice, and mouse-like devices such as lightguns, spinners, steering wheels, etc.
- **Joypad Drivers** provide access to gamepads and joysticks.

**Absolute mouse devices** in the tables below refers to input drivers which support mouse-like devices such as light guns, air mice, and Wiimotes that use 'absolute' coordinate systems. Certain input drivers only support mouse devices with 'relative' coordinate systems.

## Linux
`udev` is the most full-featured Input Driver and Joypad Driver for Linux.

**Linux Input Drivers**

- linuxraw
- sdl2
- udev
- wayland

**Linux Joypad Drivers**

- hid
- linuxraw
- sdl2
- udev
- xinput

### udev input driver
udev is the newest input driver and uses the evdev joypad interface at `/dev/input`. It supports hotplugging and force feedback (if supported by device). udev reads evdev events directly and supports keyboard callback, mice, and touchpads. `libudev` is used to discover devices and support hotplugging.

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| Yes         |  Yes          |

#### Required packages
TThe `libudev` and `libxkbdcommon` packages are required. udev does not require X, but udev does depend on X11 keyboard layout files being installed.

#### Setting up udev permissions
Most Linux distributions prevent users from capturing keyboard/mouse information by default. Only root and users in the group "input" are able to access raw input. This is a security feature in case the system is used by multiple users.

The easiest way to gain access to this input is to:

* **Step 1:** Add your user to the group "input" with the command: ``sudo usermod -a -G input `whoami` ``
* **Step 2:** Log out, and then log back in

If adding your user to the input group does not succeed, you may also set up a udev rule which makes this input accessible to non-root users:

* **Step 1:** Add to `/etc/udev/rules.d/99-evdev.rules` the following text: `KERNEL=="event*", NAME="input/%k", MODE="666"`
* **Step 2:** Reload the rules with `sudo udevadm control --reload-rules`.
* **Step 3:** Reboot

### linuxraw input driver
The older linuxraw driver is available which uses the legacy joystick API at `/dev/input/js*`. The  linuxraw driver requires an active TTY in order to read keyboard events.

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| No          |  Yes          |

### wayland input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| -           |  -            |

### sdl2 input driver

#### Features

| Multi-mouse | Absolute mice* |
|-------------|----------------|
| No          |  No            |


### hid joypad driver

#### Features

| Rumble |
|--------|
| -      |

### linuxraw joypad driver

#### Features

| Rumble |
|--------|
| -      |


### sdl2 joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

### udev joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

### xinput joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

---

## Windows

**Windows Input Drivers**

- dinput
- raw
- sdl2

**Windows Joypad Drivers**

- dinput
- hid
- sdl2
- xinput

### raw input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| Yes         |  Yes          |


### dinput input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| No          |  No           |

### sdl2 input driver
-To be written-

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| -           |  -            |

### dinput joypad driver

#### Features

| Rumble |
|--------|
| No    |

### hid joypad driver

#### Features

| Rumble |
|--------|
| -      |

### sdl2 joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

### xinput joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

---

## Android

**Android Input Drivers**

- android
- linuxraw
- udev

**Android Joypad Drivers**

- android
- hid
- udev

### android input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| -           |  -            |

### linuxraw input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| No          |  Yes          |

### udev input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| Yes         |  No           |


### android joypad driver

#### Features

| Rumble |
|--------|
| -      |

### hid joypad driver

#### Features

| Rumble |
|--------|
| -      |

### udev joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

## OS X

**OS X Input Drivers**

- cocoa

**OS X Joypad Drivers**

- hid

### cocoa input driver
-To be written-

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| -           |  -            |

### hid joypad driver

#### Features

| Rumble |
|--------|
| -    |

### sdl2 joypad driver

#### Features

| Rumble |
|--------|
| Yes    |

---

## DOS


### DOS input driver

#### Features

| Multi-mouse | Absolute mice |
|-------------|---------------|
| -           |  -            |

### DOS joypad driver

#### Features

| Rumble |
|--------|
| -    |
