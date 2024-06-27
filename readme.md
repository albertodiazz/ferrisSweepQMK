A usable default keymap for the Ferris keyboard
===============================================

The Ferris Sweep keyboard is my default keyboard for daily use. Here is the detailed layout configuration:

What do all these layers do?
----------------------------

### Layer 0: Base layer

![Layer 0](https://github.com/albertodiazz/ferrisSweepQMK/blob/main/img/layer0.png)

### Layer 1: Mouse

![Layer 1](https://github.com/albertodiazz/ferrisSweepQMK/blob/main/img/layer1.png)

### Layer 2: Navigation

![Layer 2](https://github.com/albertodiazz/ferrisSweepQMK/blob/main/img/layer2.png)

How to flash for Arch Linux?
----------------------------

```
pacman -S qmk

qmk config

# Two separate commands
# You need to put in bootloader mode your ferris

qmk flash -kb ferris/sweep -km default -bl avrdude-split-left 
qmk flash -kb ferris/sweep -km default -bl avrdude-split-right

```
Remeber the JSON you get from [QMK Configurator](https://config.qmk.fm/#/ferris/sweep/LAYOUT_split_3x5_2) needs to be placed inside the folrder `~/qmk_firmware/keyboards/ferris/keymaps/default` and replace the `keymap.json`. 
