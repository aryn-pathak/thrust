---
title: "Thrust FPV stunt drone"
author: "aryan"
description: "a visually stunning FPV Stunt drone, with a custom FC"
created_at: "2025-06-23"
---

## DAY ONE

The drone should have the following qualities:
 - Small
 - agile (speed and quick turns)
 - have a custom FC
 - cameraaa
 - be resistant to crashes (or be designed to break in a way that it can be reassembled)
 - be under $150
 - look polished and visually striking (hoping to win highway design competition :3)
 - self stabilised
 - collision prevention (to some extent)

I also need to somehow make it in 3 days to be eligible for the competition :heavysob:, but i'm still gonna make it good

Today I'll start the flight controller PCB. I was confused between using STM32F4 chips (used most commonly in drones, great perfomance) and RP2040 (slower, but easier to setup). ChatGPT said STM32 chips are significantly harder to setup initially, but post talkuing to a few people on the slack, STM isn't too hard to setup, so I'll be using the [STM32F401CCU6](https://robu.in/product/stm32f401ccu6-stmicroelectronics-stm32f401ccu6-arm-mcu-dynamic-efficiency-line-stm32-family-stm32f4-series-microcontrollers-arm-cortex-m4/) with USB FS and STMDuino support.

## DAY TWO
Made most of the schematic today
![Screenshot 2025-06-25 at 12 27 38 AM](https://github.com/user-attachments/assets/d93b4d7b-1e77-4170-934d-28e79e8750b9)
This is mostly the low level stuff for the STM32 chip to work, and added ICM-42688-P. I'll be using an ESP32-CAM module for the camera and wireless connectivity. The camera is fully independent of the STM32, and a UART connection between ESP and STM32 is used for controls.

I don't think I'll be able to submit for the design competition :sob:, but that gives me more time to work on a well designed, high perfomance drone with a custom FC.

Tomorrow, I'll get started on BOM (battery, motors, ESCs, etc), and hopefully also finish the PCB!

## DAY THREE-FOUR
Worked more on the schematic, and finally finished it!
![Screenshot 2025-06-29 at 12 38 36 AM](https://github.com/user-attachments/assets/afa290a7-e2d9-4549-9d14-ea244fa5a3ea)

It's not exactly neat, but I'll organise and label the blocks later (when i ship it).

Also, a problem i realised when going to make the PCB-- I didn't label the capacitors' and resistors' capacitance and resistance respectively :skull:, so it'll take some more time.
