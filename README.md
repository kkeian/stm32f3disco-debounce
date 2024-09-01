# stm32f3disco-debounce
Two sided switch with hardware debouncing solution provided external to the computer board.

My math may be wrong. Check it yourself.

## Schematic
Schematic was created using [Circuit-Diagram](https://www.circuit-diagram.org) free circuit diagram drawing tool.
![alt text](https://github.com/kkeian/stm32f3disco-debounce/blob/main/images/schematic.png)

Schematic drawing was model almost exactly off of the schematic for SPST switch in this great article on [hardware debounce](https://www.digikey.com/en/articles/how-to-implement-hardware-debounce-for-switches-and-relays) at DigiKey written by Clive "Max" Maxfield.

## The Circuit Components
![alt text](https://github.com/kkeian/stm32f3disco-debounce/blob/main/images/components.JPG)
The embedded board is an STM32F3-Discovery board.

## The Assembled Circuit
![alt text](https://github.com/kkeian/stm32f3disco-debounce/blob/main/images/connections0.JPG)
![alt text](https://github.com/kkeian/stm32f3disco-debounce/blob/main/images/connections1.JPG)
![alt text](https://github.com/kkeian/stm32f3disco-debounce/blob/main/images/connections2.JPG)

Firmware uses:
- an internal pull-down resistor for the blue USER button on the PCB.
- an internal pull-up resistor for Pin 1 on GPIO A (PA1 GPIO pin header).