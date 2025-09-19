# Reflow Oven Controller

A solder reflow oven controller project for Arduino Mega 2560, featuring a touchscreen interface and precise temperature control using a thermocouple.

## Overview

This project provides automated control for a solder reflow oven with configurable temperature profiles for different soldering stages (preheat, soak, reflow, cooldown). The system uses a PID controller for precise temperature management and displays real-time temperature data and reflow profiles on a touchscreen display.

## Features

- **Touchscreen Interface**: Interactive control using Adafruit HX8357 display with touch capability
- **Thermocouple Temperature Sensing**: Accurate temperature measurement using MAX31856 thermocouple amplifier
- **PID Temperature Control**: Precise temperature regulation with configurable PID parameters
- **Customizable Reflow Profiles**: Adjustable temperature and timing parameters for different solder types
- **Real-time Monitoring**: Live temperature plotting and status display
- **Safety Features**: Temperature limits and monitoring for safe operation

## Hardware Requirements

- Arduino Mega 2560
- Adafruit HX8357 TFT Display with touchscreen
- MAX31856 Thermocouple Amplifier
- K-Type Thermocouple
- Solid State Relay (SSR) for oven control
- Reflow oven or toaster oven modification

## Software Dependencies

This project uses PlatformIO and includes the following libraries:
- Adafruit MAX31856 library
- Adafruit GFX Library
- Adafruit HX8357 Library
- Adafruit TouchScreen
- PID_v1 (PID controller)
- Standard Arduino libraries (SPI, Wire, etc.)

## Installation

1. Clone this repository
2. Open the project in PlatformIO (VS Code extension recommended)
3. Build and upload to your Arduino Mega 2560
4. Connect the hardware according to the pin definitions in the code

## Pin Configuration

- Thermocouple CS: Pin 8
- SSR Control: Pin 2
- TFT CS: Pin 10
- TFT DC: Pin 9
- Touch Screen: Pins A0, A1, 6, 7

## Usage

1. Power on the system
2. Use the touchscreen interface to configure temperature profiles
3. Start the reflow process
4. Monitor temperature and progress on the display
5. System will automatically control oven temperature through the programmed profile

## Credits

**Original Project**: This project is based on the excellent work by **Zach Hipps** and **DigiKey**. 

**Original Repository**: [https://github.com/bytesizedengineering/Solder-Reflow-Oven](https://github.com/bytesizedengineering/Solder-Reflow-Oven)

**Migration Note**: This version has been migrated from the original Arduino IDE project to **PlatformIO** for improved dependency management and development workflow.

## License

Please refer to the original project licensing terms from DigiKey and Zach Hipps.

## Safety Warning

⚠️ **IMPORTANT**: This project involves high temperatures and electrical modifications to appliances. Use appropriate safety precautions, ensure proper ventilation, and verify all electrical connections. The authors are not responsible for any damage or injury resulting from the use of this project.

## Contributing

Feel free to submit issues and enhancement requests. Please ensure any modifications maintain the safety and reliability of the temperature control system.