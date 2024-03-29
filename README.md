# Ender 5 Plus
This repo contains the modifications and current configuration files for my Creality Ender 5 Plus.

## Main Board
The main board in this printer is an BTT Octopus Pro (F446).

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

Photos of cable are available here: https://imgur.com/a/O3nix8B

## Extruder
Stock

## Bed Heater
Stock

## Build Plate
Stock

## BLTouch
Stock

## Part Cooler
Stock

## Hotend Cooler
Stock cooler, but klipper has been configured so that the fan only turns on when the temperature is set to 50°C or above. When the hot end turns off, the fan turns off once the temperature drops back below 50°C.

## Enclosure Fan
The stock enclosure fan was always on and very loud, so it was replaced with a 5V Noctua fan. It is connected to the Octopus via one of the fan ports which is set to 5V. It turns on and off automatically whenever the extruder or bed are turned on.

## Firmware
Klipper is loaded onto this printer, see [printer.cfg](printer.cfg)

It is running on a Raspberry Pi 4B mounted inside the control box using the [3D printed mount found here](Ender5Plus-Octopus-and-Pi-Mount.stl).
