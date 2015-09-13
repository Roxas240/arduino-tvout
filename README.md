The goal of this project is to create a simple interupt driven library for generating composite video on a single AVR chip.

Currently the output is NTSC or PAL at a resolution of 128x96 by default. The library currently works on ATmega168,328,1280,2560,644p,1284p,AT90USB1286 and more can be added by editing one file.

# News

Beta1 for version 1.0 is out!!! It has some it changes the hardware connections as well as some of the function calls see the wiki for full details.

# Connections

![connection](http://xemplar.ml/media/hosted/5225072558_5f5f760037.jpg)

SYNC is on OCR1A and AUDIO is on OC2A

There are some timing issues with the m1284p, may be related to sanguino core.

|MCU        | SYNC | VIDEO | AUDIO | Arduino       | SYNC | VIDEO | AUDIO |
|-----------|------|-------|-------|---------------|------|-------|-------|
|m168,m328  |B1    |D7     |B3     |NG,Decimila,UNO|9     |7      |11     |
|m1280,m2560|B5    |A7     |B4     |Mega           |11    |A7(D29)|10     |
|AT90USB1286|B5    |F7     |B4	   |--             |--    |--     |--     |

# Products Based on TVout

Wayne and Layn LLC now makes a shield that uses this library, the video game shield.
nootropic design is selling a stand alone arduino compatible board the hackvision.

# Included Examples

Very simple as they may be.

[![TVout 1.0 Beta1 Demo](http://img.youtube.com/vi/MEg_V4YZDh0/0.jpg)](https://www.youtube.com/watch?v=MEg_V4YZDh0 "TVout 1.0 Beta1 Demo")
[![Arduino Tetris](http://img.youtube.com/vi/bHpFv_x_8Kk/0.jpg)](https://www.youtube.com/watch?v=bHpFv_x_8Kk "Arduino Tetris")

