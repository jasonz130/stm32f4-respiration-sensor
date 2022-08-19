# stm32f4-respiration-sensor
Programmed the STM32F429 microcontroller to detect respiration rate and amplitude, with the use of HAL libraries. Two sensors, Hall effect sensor and the IR photodiode were implemented to detect
respiration rate. In the event the Hall effect sensor fails to detect any changes to respiration rate, the IR photodiode will activate and act as the substituting sensor.

The code in Core/Src/main.c works in 3 segments. 
Part 1 is the ideal case where the Hall effect sensor works as intendence.
Part 2 initiates when the Hall effect sensor fails to detect respiration rate. This activates the IR photodiode sensor.
Part 3 initiates when both sensors fails to detect respiration rate.

The hardware schematic is provided in the folder Schematic.
