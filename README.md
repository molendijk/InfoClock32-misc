# InfoClock32-misc

## Introduction
This repository contains miscellaneous files useful in conjunction with the infoclock32 as developed by Bartek:
https://github.com/bartoszbielawski/infoclock32
Many thanks to Bartek who initially created such a clock for the ESP8266 microcontroller quite some years ago and now took the project one step further by using the ESP32 controllers enabling much more nice features as the initial infoclock.
Please refer to the link above for the detailed description of this project with sources and generated target code for four popular variants of the ESP32 family.

## 3D printing
The supplied CAD files, stl files and Creality 3D project files allow to 3D print a case for the infoclock32 using the ESP32-C3 (SuperMini) micro controller.
It is not necessary to use the Creality projects, published here, if you want to use another 3D printing environment, just import the stl files in the slicer that comes with your 3D printer.

I have created these CAD files using FreeCAD version 1.1. The InfoClock_Body.FCStd files have been designed fully parametrically using a spreadsheet to dynamically enable modifying the design with minimal chance of breaking it.
I have tested these designs using hyper PET-G printed on a low-cost Creality K1SE 3D printer without any assembly issues.

## Assembly
The clock body is printed as 2 equal parts that are designed to be pressed together forming a compact enclosure.
The two assembles parts can then be solidly attached using two (270mm long) M3 threads and M3 nuts.
The main clock body was also designed to optionally support the use of a 3mm plexiglass optical display filter to enhance the display contrast. The 3mm thick filter dimensions should measure 34 x 266mm for a good fit.
You should select a type of plexiglass with a fairly high optical transmission factor with a color that matches that of the display modules used.

## Some details
The clock uses two cascaded, 4 module MAX7219 LED dot matrix display modules driven over an SPI bus by the microcontroller.
Note: the display is powered by a 5V supply in contrast to the optional (i2c) sensor modules that all use 3.3V.

## Disclaimer
In spite of my efforts to create a useful 3D printable project for the infoclock32 (variant ESP32-C3), I cannot guarantee that the margins I used will generate a fitting (usable) design using your 3D printer with your filament used.
