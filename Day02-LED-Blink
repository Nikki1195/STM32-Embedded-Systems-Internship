# Day 2 - GPIO LED Blink

## Objective

Learn GPIO configuration and create the first STM32 program to blink an LED using STM32CubeIDE and PICSimLab.

## Hardware / Simulator

- STM32F103C8T6 (Blue Pill)
- PICSimLab
- STM32CubeIDE

## Concepts Learned

- GPIO Output Mode
- STM32 HAL Functions
- Digital Output Control
- Delay Generation

## GPIO Pin Used

| Pin | Function |
|------|----------|
| PB8 | LED Output |

## HAL Functions Used

```c
HAL_GPIO_WritePin();
HAL_GPIO_TogglePin();
HAL_Delay();
```

## Program Flow

1. Configure PB8 as GPIO Output.
2. Turn LED ON.
3. Delay 500 ms.
4. Turn LED OFF.
5. Delay 500 ms.
6. Repeat forever.

## Code Snippet

```c
while (1)
{
    HAL_GPIO_TogglePin(GPIOB, GPIO_PIN_8);
    HAL_Delay(500);
}
```

## Result

LED successfully blinks every 500 ms in PICSimLab.

## Learning Outcome

Successfully created and executed the first STM32 firmware application using GPIO output and HAL APIs.
