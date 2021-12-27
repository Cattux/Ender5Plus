# Ender 5 Plus
This repo contains the modifications and current configuration files for my Creality Ender 5 Plus.

## Main Board
The main board in this printer is an BTT SKR-Mini E3 V2.0.

## Screen
The screen is still the stock screen. A custom cable was created so that it could work with the new main board via the TFT pins, see pinout below:

| LCD Pin | SKR Pin | Description        |
| ---     | :--     | :--                | 
| 1       | 5       | 5V                 | 
| 2       | NC      |                    | 
| 3       | 3       |  LCD RX / SKR TX2  | 
| 4       | 2       | LCD TX / SKR RX2   | 
| 5       | NC      |                    | 
| 6       | 4       | GND                | 

## Extruder
Stock

## Bed Heater
Stock

## Build Plate / Y Carriage
Stock

## BLTouch
Stock

## Part Cooler
Stock

## Hotend Cooler
Stock

## Firmware
Klipper is loaded onto this printer, see [printer.cfg](printer.cfg)

It is running on a Raspberry Pi 4B. Currently it is just sitting beside the printer, but will soon be mounted inside of the control box and powered from the SKR with a DCDC converter to drop the voltage to 5V.
