# Day 3 - ADC and UART Communication

## Objective

Configure STM32 ADC channels to read analog sensor values and transmit the readings through UART using STM32 HAL and PICSimLab.

## Hardware / Simulator

* STM32F103C8T6 (Blue Pill)
* STM32CubeIDE
* PICSimLab
* Virtual Terminal (UART)

## ADC Channel Mapping

| Pin | Function              |
| --- | --------------------- |
| PA0 | Accelerator           |
| PA1 | Brake                 |
| PA2 | State of Charge (SOC) |
| PA3 | Temperature           |

## UART Configuration

* USART1
* Baud Rate: 115200 bps
* Mode: Asynchronous

## Features Implemented

* Configured ADC1 channels IN0-IN3
* Read four analog inputs using potentiometers
* Displayed ADC values through UART terminal
* Verified real-time sensor updates in PICSimLab

## Sample Output

ACC=655 BRAKE=983 SOC=2047 TEMP=1269

## Learning Outcomes

* ADC configuration using STM32CubeMX
* Multi-channel analog data acquisition
* UART communication using HAL drivers
* PICSimLab analog sensor simulation

## Result

Successfully acquired analog sensor data from four channels and transmitted the values over UART to a virtual terminal.
