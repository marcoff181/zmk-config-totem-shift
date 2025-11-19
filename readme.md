# My ZMK config for the TOTEM-SHIFT split keyboard
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="keymap-drawer/totem.svg">
  <source media="(prefers-color-scheme: light)" srcset="keymap-drawer/totem.svg">
  <img alt="keymap">
</picture>

My personal keymap, which includes:

- Home row mods
- Mouse emulation
- Combos for Enter/Tab
- Caps words
- Avoids usage of inner thumbs for comfort
- Support for accented vowels with composition:  ``` ` + e = è```
- Volume, Media, Brightness and Bluetooth controls


## What is the TOTEM-SHIFT?
TOTEM-SHIFT is a modified 38 keys column-staggered split keyboard [originally created by GEIGEIGEIST](https://github.com/GEIGEIGEIST/totem) and then modified by [Endracion](https://github.com/Endracion/), running [ZMK](https://zmk.dev/). It's meant to be used with a SEEED XIAO BLE. [Here](https://github.com/Endracion/TOTEM-SHIFT) are the updated TOTEM-SHIFT hardware files.

It includes these additional projects:
- caksoylar's [RGB LED Widget](https://github.com/caksoylar/zmk-rgbled-widget)
- carrefinho's [Prospector Dongle along with tokyo2006's nice!nano v2 compatibility](https://github.com/tokyo2006/prospector-zmk-module/tree/support_nicenano)


## Usage

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the totem.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the TOTEM to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `totem_left-seeeduino_xiao_ble-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the `totem_right-seeeduino_xiao_ble-zmk.uf2` file.
