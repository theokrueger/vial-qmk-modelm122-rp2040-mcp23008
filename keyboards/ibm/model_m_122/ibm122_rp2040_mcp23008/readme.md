# ibm122m_rp2040_mcp23008

![IBM Model M 122 key](https://i.imgur.com/Oo3Ozqz.jpg)

This is a keymap for the IBM Model M 122 key terminal keyboard running on the RP2040.
It is intended as a full PCB replacement, with vial support.
Since the M122 requires more pins than the RP2040 has, you are intended to use 2x MCP23008 GPIO expanders and an RP2040-Zero.

* Keyboard Maintainer: [theokrueger](https://gitlab.com/theokrueger)
* Hardware Supported: RP2040
* Hardware Availability: https://www.raspberrypi.com/products/rp2040/

Pins of the RP2040 board you should use by default:
```  
Columns: 1  2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20  
Pins:    0  1  2  3  4  5  6  7  8  9  10 11 B7 B6 B5 B4 B3 B2 B1 B0
--------------------------------------------------------  
Rows: 1  2  3  4  5  6  7  8  
Pins: A7 A6 A5 A4 A3 A2 A1 A0
--------------------------------------------------------  
Status LEDs: CapsLock +5V ScrollLock NumLock  
Pins:        N/A      5V  N/A        N/A
```

Make example for this keyboard (after setting up your build environment):

    make ibm/model_m_122/ibm122m_rp2040_mcp23008:vial

See [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) then the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information.
