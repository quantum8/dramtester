# Dramtester V 4.2.1 by Mirco Gaggiottini
Dram tester for 4116 and 4164/256 (now in beta testing for 4532)

Simple project taken from the base of @FozzTexx

with added support for 4116 memories and a status display.

This Tester supports 4164,41256,4116,*4532* and pin compatible Dram.

![alt text](https://github.com/zeus074/dramtester/blob/main/IMG/IMG_6060.jpg)

:coffee: if you want the PCB, please support me and follow this link : <a href="https://www.pcbway.com/project/shareproject/Dram_tester_for_4116_4164_256_and_4532_d6b7143c.html" target="_NEW">PCBWAY!</a>

**Components:**

C1,C4,C5,C6,C7: 100nF

C2: 10uF 25v

C3: 47uf 25v

D1: BAT43 (optional, you can short)

DC: MT3608 (DC-DC converter - 4~5V in, 12V out)

Disp: Display oled 128x32 i2c

H1,H2,H3: 3 pin Header-Male 2.54

R1-R13: 47 Ω 1/8w (optional)

R14,R16: 10k Ω 1/4w

R15: 2.2k Ω 1/4w

1x Arduino Nano

1x Zif 16 pin (or 16 pin socket)

1x 7760 (7660s)

1x tactile switch 6x6

N.B.: The DC-DC must be able to accept 4V on input and must be set to output 12V


**Directory**

Gerber : https://www.pcbway.com/project/shareproject/Dram_tester_for_4116_4164_256_and_4532_d6b7143c.html

IMG : Tester's pictures

Firmware : Firmware for Arduino Nano (you can use avr commands like Arduino's IDE or an AVR programmer to write the HEX file)


**How it works**

First you need to flash the firmware on arduino of course!.

Before inserting the ram select the correct setting with the jumpers: (all jumpers must be in the same position, all high for 4164 or all low for 4116)

![alt text](https://github.com/zeus074/dramtester/blob/main/IMG/jumper_positions.jpg)


If the setting is on 4164-256 it is possible to select the type of memory (from 4164,41256,4532-L,4532-H) by briefly pressing the select / start key.
(memory 4116 has no selections)

To start the test, keep the select / start key pressed for 1 sec.

After the test the result will be displayed, if there is an error the test will stop and the point of the error will be shown.

**How to burn the firmware**

You can use avrdude integrated on arduini via command line, or simply download a gui (if you use windows) like AVRDUDESS.
![alt text](https://github.com/zeus074/dramtester/blob/main/IMG/programming.JPG)

**Support 3D Print**

Thanks to seanch80, you can print the base in 3D, the stl file is in the 3D_print folder.
![alt text](https://github.com/zeus074/dramtester/blob/main/IMG/base_3D.jpg)

You will also find a "3jumpers" file to be able to glue the 3 jumpers in order to easily move them all together.
![alt text](https://github.com/zeus074/dramtester/blob/main/IMG/3jumpers.jpg)
