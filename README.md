# STM32 Flight Controller

Open-source STM32F405 flight controller designed in EasyEDA Pro.

## Specs

| | |
|---|---|
| **MCU** | STM32F405RGT6 (168 MHz, 1 MB flash), 8 MHz crystal |
| **IMU** | TDK ICM-42688-P |
| **Barometer** | Infineon DPS368 |
| **Blackbox flash** | W25Q128JV (16 MB) |
| **Power** | MP9943 buck regulator + 2× TPS7A20 3.3 V LDOs, resettable fuse |
| **USB** | USB-C with USBLC6-2 ESD protection |
| **Connectors** | JST-SH 8-pin (ESC), JST-SH 6-pin, solder pads for motors M1–M4, VBAT, current sensor, RX/TX, 5 V |
| **Other** | Boot button, status LEDs |
| **PCB** | 6 layers (4 inner), blind/buried vias |

## Files

| File | Description |
|---|---|
| `hardware/Flight Controller.epro2` | EasyEDA Pro project (schematic + PCB) |
| `hardware/Schematic.pdf` | Schematic, viewable without EasyEDA |
| `hardware/BOM.xlsx` | Bill of materials |
| `hardware/PickAndPlace.xlsx` | Component placement file for SMT assembly |
| `hardware/Gerber.zip` | Gerber and drill files for manufacturing |

## Ordering the PCB

1. Upload `hardware/Gerber.zip` to [JLCPCB](https://jlcpcb.com) (or any PCB fab).
2. Select 6 layers.
3. For assembly, enable **PCB Assembly** and upload `BOM.xlsx` and `PickAndPlace.xlsx`.

## Opening the design

Open [EasyEDA Pro](https://pro.easyeda.com), then **File → Import → EasyEDA Pro** and select `Flight Controller.epro2`.

## Status

🚧 Untested / work in progress.

## License

MIT
