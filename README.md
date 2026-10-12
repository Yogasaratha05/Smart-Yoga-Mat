# Smart-Yoga-Mat
A smart yoga mat prototype using a load cell, HX711 amplifier, Arduino, and I2C LCD to measure applied weight and suggest yoga poses based on predefined weight ranges.
# Load Cell-Based Smart Yoga Mat

## Project Description

The Smart Yoga Mat is an embedded system prototype designed to measure the weight applied to a mat using a load cell and HX711 24-bit ADC module.

The measured value is displayed on a 16x2 I2C LCD. Based on predefined weight ranges, the system suggests different yoga poses.

## Objectives

* Measure applied load using a load cell.
* Process sensor signals using the HX711 module.
* Display weight readings on an LCD.
* Demonstrate rule-based yoga pose suggestions.

## Hardware Components

* Arduino-compatible microcontroller
* Load cell
* HX711 load cell amplifier module
* 16x2 I2C LCD display
* Connecting wires
* Power supply

## Software Requirements

* Arduino IDE
* HX711_ADC library
* LiquidCrystal_I2C library
* EEPROM library, if required by the selected board and configuration

## Features

* Load cell data acquisition
* Weight display on LCD
* Serial Monitor output
* Weight-range-based yoga pose suggestions
* Tare function through the Serial Monitor

## Working Principle

1. The load cell senses an applied load.
2. The HX711 module converts the load cell signal into digital data.
3. The microcontroller reads the processed data.
4. The measured value is displayed on the LCD.
5. A predefined rule selects a yoga pose suggestion according to the configured weight range.

## Yoga Pose Selection

* 20–40: Vajrasanam
* 40–80: Badmasanam
* 80–100: Sirasasanam

These ranges follow the example code and must be verified against the intended units and application.

## Limitations

* The calibration value must be adjusted for the actual load cell and setup.
* The code multiplies the sensor reading by 100; the resulting value is not guaranteed to represent grams without proper calibration.
* Yoga poses are suggested using weight thresholds only; this does not assess posture or determine whether a pose is safe for a person.

## Future Enhancements

* Improve sensor calibration and weight accuracy.
* Add posture detection sensors.
* Display instructions for yoga poses.
* Add Bluetooth or Wi-Fi connectivity for monitoring.
* Develop a mobile application for progress tracking.

## Project Status

Prototype implementation — calibration and hardware testing required.

## Disclaimer

This project is intended for educational purposes. Yoga pose suggestions are not medical or personalized exercise advice.

