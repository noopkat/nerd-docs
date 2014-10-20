# SPI docs

### in depth

+ [http://en.wikipedia.org/wiki/Serial_Peripheral_Interface_Bus](http://en.wikipedia.org/wiki/Serial_Peripheral_Interface_Bus)
+ [http://avrbeginners.net/architecture/spi/spi.html](http://avrbeginners.net/architecture/spi/spi.html)
+ [https://sites.google.com/site/qeewiki/books/avr-guide/spi](https://sites.google.com/site/qeewiki/books/avr-guide/spi)

### what arduino does

+ [https://github.com/arduino/Arduino/blob/master/libraries/SPI/SPI.cpp](https://github.com/arduino/Arduino/blob/master/libraries/SPI/SPI.cpp)
+ [http://arduino.cc/en/Reference/SPITransfer](http://arduino.cc/en/Reference/SPITransfer)

### arduino suggesting to write your own
+ [http://arduino.cc/en/Tutorial/SPIEEPROM](http://arduino.cc/en/Tutorial/SPIEEPROM)

### nerdnerdnerdthings
+ [http://garretlab.web.fc2.com/en/arduino/inside/arduino/Arduino.h/digitalPinToBitMask.html](http://garretlab.web.fc2.com/en/arduino/inside/arduino/Arduino.h/digitalPinToBitMask.html)
+ [http://garretlab.web.fc2.com/en/arduino/inside/arduino/Arduino.h/portOutputRegister.html](http://garretlab.web.fc2.com/en/arduino/inside/arduino/Arduino.h/digitalPinToBitMask.html)

![port mappings](http://cl.ly/image/3L2m0W1e1s2O/Screen%20Shot%202014-10-19%20at%2014.59.26%20.png)

### beaglebone bro
+ [https://github.com/TJC/BeagleBone/blob/master/doc/SSD1306.txt](https://github.com/TJC/BeagleBone/blob/master/doc/SSD1306.txt)

### bitwise explanation is always handy for this stuff
+ [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators)

### extended firmata

+ https://github.com/kraman/go-firmata/blob/master/contrib/ExtendedFirmata/ExtendedFirmata.ino
+ firmata SPI PR - https://github.com/firmata/arduino/pull/135

### microview pins and info

```
#define CLK 13
#define MOSI  11
```
Clk pin is digital pin 13  
Mosi pin is digital pin 11

```
#define DCPORT  PORTB
#define DCDDR DDRB
#define DCBIT 0
```
which would mean that dc is digital pin 8

```
#define RESETPORT PORTD
#define RESETDDR  DDRD
#define RESETBIT  7
```
which would mean that reset is digital pin 7

```
#define SSPORT  PORTB
#define SSDDR DDRB
#define SSBIT 2
```
which would mean that slave select is digital pin 10
