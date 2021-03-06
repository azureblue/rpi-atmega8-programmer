# avr-spi-programmer
### Simple ATmega* / ATtiny* flash programmer for Raspberry Pi (and probably other devices supporting SPI sysfs and GPIO sysfs).

It uses **SPI** (3 wires directly connected to the microcontroller), **GPIO** (one pin (default 21), connected to the MCU RESET pin) and of course common ground. **The microcontroller must be powered with 3.3v**.

In this configuration the MCU can be powered from the 3.3v RPi line probably (I mean, only the microcontroller itself. If you draw more power from the 3.3v RPi line (like more than 50mA) you can fry you RPi).

**Do not use 5v as it would probably damage the RPi!**

Currently supported models include:
- ATmega8*
- ATmega48A/PA/88A/PA/168A/PA/328/P
- ATtiny85/45/25
