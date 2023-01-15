# Milestone3.2: stm32basicinterfacing
Group Name: **Lucky Lizard** :lizard:

Group Member: 
1. **Andi Nur Asyikin Binti Andi Zainuddin**
2. **Lim Yong Chuan**
3. **Nur Fatini Binti Isa**

## Ojective
Interface the UART and one more devices using the STM32F4 ports
## Equipment
- [x] Board used: **NUCLEO-F411RE**
- [x] Software used: **STM32CubeIDE**
- [x] Breadboard
- [x] Jumper
- [x] INMP441 omnidirectional MEMS microphone
## Software
- [x] PuTTY
## Procedure
1. In this milestone, the PuTTY terminal is used as the output display of the board with INMP441 MEMS microp.
2. The source code [stm32helloworld.c](https://github.com/LuckyLizard-MKEL1123/stm32helloworld/blob/main/stm32helloworld.c)
3. The microphone module has 3 main pins whic are the VCC, VDD ad data which are connected to the board.
4. The 3 data pins are the I2S2 WS, SD and CK which are connected to the PB11, PB12 and PC3 of the STM32F411RE board.
5. The interfacing of the microphone module is done using the I2S (Inter-IC Sound) protocol whic is provided by the STM32 Cube IDE
6. The I2S data transfer is executed using a HAL function, HAL_I2S_Receive() to receive the microphone data.
7. Once sound is detected, a message 'Sound detected' will be displayed on the PuTTY terminal.

## Results
Link for the video demo: [stm32basicinterfacing] (https://youtu.be/90DmdmSMC6Y)

## References
1. https://deepbluembedded.com/stm32-debugging-with-uart-serial-print/
2. https://elearning.utm.my/22231/pluginfile.php/505626/mod_resource/content/0/10-serial%20communications%20.pdf
