---
title: "Thrust FPV stunt dront"
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

Today I'll make the flight controller PCB. I was confused between using STM32F4 chips (used most commonly in drones, great perfomance) and RP2040 (slower, but easier to setup). ChatGPT said STM32 chips are significantly harder to setup initially, but post talkuing to a few people on the slack, STM isn't too hard to setup, so I'll be using the [STM32F401CCU6](https://robu.in/product/stm32f401ccu6-stmicroelectronics-stm32f401ccu6-arm-mcu-dynamic-efficiency-line-stm32-family-stm32f4-series-microcontrollers-arm-cortex-m4/) with USB FS and STMDuino support.
