# SC16IS752

I forked from [here](https://github.com/TD-er/SC16IS752)   

Added: Constructor Overload to accept other instances of I2C or SPI. (in my project I needed to use SPI3).

Example:

#include <SPI.h>

#include <SC16IS752.h>

SPIClass spi3(SPI3_MOSI,SPI3_MISO,SPI3_SCK);

SC16IS752 Bridge( &spi3 ,SS_pin);

