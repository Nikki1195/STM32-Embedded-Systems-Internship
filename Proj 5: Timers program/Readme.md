# STM32 TIM1 LED Blink Using Interrupt

## Overview

This project demonstrates LED blinking using the TIM1 timer interrupt on the STM32F103C8T6 (Blue Pill) microcontroller. The LED connected to PC13 toggles automatically every one second without using delays inside the main loop.

## Features

* Timer interrupt based LED blinking
* Uses STM32 HAL Library
* Configured using STM32CubeMX
* Developed in STM32CubeIDE
* Simulated using PICSimLab

## Hardware Required

* STM32F103C8T6 (Blue Pill)
* ST-Link Programmer (for real hardware)
* USB Cable
* PC/Laptop

## Software Required

* STM32CubeIDE
* STM32CubeMX
* PICSimLab (for simulation)

## Pin Configuration

| Pin  | Function        |
| ---- | --------------- |
| PC13 | LED Output      |
| TIM1 | Timer Interrupt |

## Timer Configuration

| Parameter    | Value   |
| ------------ | ------- |
| Timer        | TIM1    |
| Prescaler    | 7199    |
| Period       | 9999    |
| Counter Mode | Up      |
| Interrupt    | Enabled |

## Working Principle

1. Initialize the STM32 peripherals.
2. Configure TIM1 with the required prescaler and period.
3. Enable TIM1 Update Interrupt.
4. Start TIM1 using `HAL_TIM_Base_Start_IT()`.
5. Every timer overflow triggers `HAL_TIM_PeriodElapsedCallback()`.
6. Inside the callback, the LED connected to PC13 is toggled.
7. The LED continues blinking every one second.

## Project Structure

```
Core
├── Inc
│   └── main.h
├── Src
│   ├── main.c
│   └── stm32f1xx_it.c
```

## Output

The LED connected to PC13 blinks every one second.

## Applications

* Learning STM32 timers
* Embedded Systems laboratory
* Interrupt programming
* Real-time embedded applications

