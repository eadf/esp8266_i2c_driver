esp8266 I²C driver

This driver has been superseded by [this I²C driver](https://github.com/eadf/esp8266_i2c_master).


I've reduced the public API of zarya's I²C driver to just  ```i2c_readRegister()```,  ```i2c_writeRegister()``` and  ```i2c_init()```.

The driver uses two arbitrary pins, just give ```i2c_init()``` the pin numbers and it will connect the dots.

* Add ```#include "i2c/i2c.h"``` to your code
* Add ```driver/i2c``` (or whatever you name this folder to) to the MODULES line in the makefile

You will also need to include the [easygpio](https://github.com/eadf/esp8266_easygpio) library to your project in the same way.
