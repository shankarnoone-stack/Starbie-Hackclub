## Starbie
Starbie is a small virtual pet PCB made with a XIAO ESP32-C3. It uses a 0.96-inch OLED screen to show an animated pet menus and different stats. The project also has two buttons, an MPU6050 motion sensor, and a DHT11 temperature and humidity sensor.

I designed the schematic and PCB in KiCad, routed the traces, and exported the fabrication files.  I also wrote the Arduino IDE code for this project. This is my Week 1 PCB project for Hack Club Half Life.


![Starbie front render](Screenshot%202026-10-22%20111526.png)
This is the PCB.
![Starbie front render](Screenshot%202026-10-11%20124137.png)

## What it is

Starbie is designed to sit on your desk and react to how you handle it. Tilting, moving, and otherwise checking in on your pet are meant to be part of the experience.

The board includes a microcontroller, display, motion sensor, and environmental sensor in a compact PCB design. It is USB powered.

## How?

I started by following the guided Starbie project from [SharKingStudios](https://github.com/SharKingStudios/Starbie ), as this was the guide to my design I was going to build.
After, I set up the schematic with the XIAO ESP32-C3, OLED display, MPU6050, DHT11 sensor, and buttons.
I also had an error with routing the footprints to the PCB, but then realized that I had to use a diffferent footprint for it to work.
After this, I routed the traces, and checked it using designs rules checker to make sure that it was ok.
I finally exported the fabrication files and BOM.

## Why?
I made it for the Week 1 Half Life hackclub challenge, to learn about how to use KiCad and build a PCB and Schematic.

## Firmware
For my code, I added a sparkle trail and added a blinking animation on top of the starter code in Arduino IDE.
## BOM.csv
I looked towards Amazon for my parts, and used JLCPCB for my PCB vendor. For my microcontroller, I first thought of aliexpress, but then I realized it was better to go with Seeed Studio.
| Part| Quantity | Price | Vendor |
|---|---:|---:|---|
| [XIAO ESP32-C3](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html)| 1 |$5| Seeed Studio |
| [0.96-inch OLED Display](https://www.amazon.com/Display-SSD1306-Self-Luminous-Compatible-Raspberry/dp/B0GBWXTR1Z)| 1 | $6 | Amazon |
| [10k Resistor](https://www.amazon.com/10K-Resistor-Tolerance-Resistors-Resistance/dp/B0B4JFPHTW)| 1 | $0.05 |Amazon|
| [Keycaps](https://www.amazon.com/dp/B0CQ2VLMVY)| 1 | $2.40 | Amazon |
| [MPU-6050](https://www.amazon.com/dp/B0943SGP34)| 1 | $2.29 | Amazon |
| [DHT11](https://www.amazon.com/dp/B0BLG7R99R) | 1 | $3.33 | Amazon |
| [MX Switches](https://www.amazon.com//dp/B0FQP8VYX4)| 4 | $0.72 | Amazon |
| [PCB Fabrication](https://jlcpcb.com/)| 1 | $8.40 | JLCPCB |

- **Parts Subtotal:** 28.19
- **Tax & Shipping:** $21.44 (Including PCB manufacturing shipping/taxes)
- **Total Project Cost:** **$49.63**

## Repository contents

- KiCad source files and fabrication exports
- PCB renders
- Arduino
- BOM
- Gerber files
