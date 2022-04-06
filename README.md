# PocketEC compatible ADUCM355 firmware

Firmware included for control of an ADUCM355 potentiostat device using the PocketEC app.

## Hardware

* EVAL-ADUCM355QSPZ
* HC-06 Bluetooth Serial Transceiver
* AD mIDAS-Link emulator

## Implementation

This code has been tested using an ADUCM355 evaluation board (EVAL-ADUCM355QSPZ) connected to a HC-06 bluetooth module.
Prepare the evaluation board by removing jumpers JP45 and JP46, then bridge JP45 to the bluetooth module RX pin, and JP46 to the TX pin.
The module may be powered by connecting pin 2 and pin 7 of the evaluation board J-TAG CONNECTOR (P27) to ground and VCC pins of the bluetooth module, respectively.

## Running the code 

The "PocketEC\iar" folder contains an IAR project that can be opened with the IAR Embedded Workbench IDE.
After connecting the board to the emulator/debugger press Download/Debug to load the firmware onto the board.
Setup the device on the PocketEC app by connecting to the HC-06 blueotooth module and selecting the JSON file for the ADUCM355 platform.
After downloading the firmware you should be able to run the device without an emulator/debugger present. 
