# mySatComm
Homebrew groundstation for receiving data from satellites

## Quick Reference
* [Controller Design](mechanical/drawings/controller.PDF)
* [Dipole Antenna Design](mechanical/drawings/controller.PDF)
* [Materials Used](BOM.txt)

## Project Breakdown
* Antenna Design
  * Linearly Polarized Yagi Antenna
  * Currently 3-element implementing a basic dipole antenna
* Az-El Controller
  * 2 servo motors control antenna orientation
  * Using Arduino and GPredict to actuate
* Data Reception
   * Using the NooElec NESDR for a radio
   * Using GNURadio to implement the needed DSP
* Decoding
   * TBD

## Software Used
SolidWorks
- Mechanical design software by Dassault Systems
- Not free; requires a license

Arduino IDE
- Used to implement motor controller
- Open source

GNURadio
- Software-Defined Radio programming package
- Free to use

GPredict
- Satellite position tracker/predicter
- Free to use

## Folder Guide
* mechanical
  - Contains all CAD designs
* cmd-n-ctl
   - Code for antenna orientation controller
   - Code for GPredict controller interfacing
* sdr
  - Code for radio interfacing