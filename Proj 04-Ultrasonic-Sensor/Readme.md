# Project 4 - Ultrasonic Sensor Interfacing

## Objective

To interface the HC-SR04 Ultrasonic Sensor with STM32F103C8T6 and measure distance using PICSimLab.

## Tools Used

* STM32CubeIDE
* PICSimLab
* STM32F103C8T6 (Blue Pill)
* HC-SR04 Ultrasonic Sensor

## Pin Configuration

| Pin | Function |
| --- | -------- |
| PA0 | Trigger  |
| PA1 | Echo     |

## Working Principle

1. A trigger pulse is sent to the HC-SR04 sensor.
2. The sensor transmits an ultrasonic wave.
3. The echo signal is received back after reflection from an object.
4. The pulse duration of the echo signal is measured.
5. Distance is calculated and displayed through UART.

## UART Configuration

* USART1
* Baud Rate: 115200
* Mode: Asynchronous

## Sample Output

Distance = 393 cm

Distance = 80 cm

Distance = 194 cm

Distance = 287 cm

## Concepts Learned

* GPIO Input and Output
* Ultrasonic Sensor Interfacing
* Pulse Width Measurement
* Distance Calculation
* UART Communication
* STM32 HAL Programming

## Result

Successfully interfaced the HC-SR04 Ultrasonic Sensor with STM32 and measured distance in PICSimLab. The calculated distance was displayed on the Virtual Terminal through UART communication.
