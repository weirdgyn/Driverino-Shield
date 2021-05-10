# Driverino 

### (italian noun) /ˈdraɪvərnəʊ/ : *little driver*

Driverino is a pretty simple, low power, driver for [BLDC](https://en.wikipedia.org/wiki/Brushless_DC_electric_motor) sensored motors.
The project target was to create a very small unit capable of driving a motor rated about 50-100W.
The board is fitted with ATmega32U4 micro the same of Arduino Micro Pro commercial boards, once the correct bootloader has been burned-in the board should act as an Arduino board (at least for programming/debugging task) and also spin a motor.
The project includes:
 1. Fully designed 2 layers PCB board (KiCAD);
 2. Driverino firmware sources;
 3. MCT8316Z library sources.

Driverino's firmware allow users to drive BLDC motors using a standard [RS232](https://en.wikipedia.org/wiki/RS-232) interface trough simple interactive commands.
The firmware allows also:
* closed loop speed control (implementing a [PID](https://en.wikipedia.org/wiki/PID_controller) loop);
* motor/driver status monitoring;
* R/C ESC emulation.

The library allows Arduino users to interact with BLDC motors without knowledge of MCT8316Z chip and [SPI](https://en.wikipedia.org/wiki/Serial_Peripheral_Interface) protocol.

## Driverino features

* ATmega32U4 microcontroller;
* Micro [USB](https://en.wikipedia.org/wiki/USB) interface;
* MCT8316Z motor driver;
* 41x26mm (size);
* RS232 interface;
* Standard R/C input compatibile.

The board can drive up to 24V-36V 8A rated sensored BLDC motors and provide 5V power supply (200mA max) mimicking R/C ESC BEC feature.
Driverino supports a variety of different types of [Hall](https://en.wikipedia.org/wiki/Hall_effect_sensor)'s sensors (analog single ended, analog differtial, digital) and also different sensors supply rates (3.3V and 5V). To correctly fit for a specific sensor kind some soldering may be required: by default the board project is fitted for digital 5V sensors.

## Firmware

TBD

## Library

TBD

# TODO:

- [ ] Add features:
   - [ ] vm measurement;
   - [ ] current measurement (via INA250).
- [ ] Optimize PCB layout.
- [ ] Write Library.
- [ ] Write Firmware.
- [ ] Submit to Kitspace
- [ ] Submit to Made-With-KiCAD

# Links

* [Atmel/Microchip ATMega32U4](https://www.microchip.com/wwwproducts/en/ATmega32U4)
* [TI MCT8316Z](https://www.ti.com/product/MCT8316Z?keyMatch=MCT8316Z&tisearch=search-everything)
* [Arduino](https://www.arduino.cc/)
* [KiCAD](https://www.kicad.org/)
