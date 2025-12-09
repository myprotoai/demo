# Wearable Air Quality Pendant 🌬️
## Circular Casing (Original Design)

A compact, battery-powered wearable device that continuously monitors air quality using TVOC detection. Get real-time feedback about your breathing environment through intuitive LED indicators and audio alerts.

## Project Overview

This DIY air quality monitor pendant uses professional-grade sensors to track Total Volatile Organic Compounds (TVOC) in real-time. Perfect for monitoring indoor air quality at home, office, or industrial environments.

### Key Features

- **Real-time TVOC monitoring** using SGP40 sensor
- **Ultra-low power design** with STM32U083KCU6 microcontroller
- **Intuitive feedback** - Color-coded LEDs and musical alerts
- **Wearable design** - Compact 32.5mm diameter circular pendant
- **All-day battery life** with efficient power management
- **Professional accuracy** with industrial-grade sensor

## Air Quality Classifications

| TVOC Level | Status  | LED Color       | Audio Alert    |
| ---------- | ------- | --------------- | -------------- |
| 0-200      | Good    | 🟢 Green        | Soft tone      |
| 201-300    | Warning | 🟡 Yellow       | Warning melody |
| 301-500    | Alarm   | 🔴 Red          | Urgent beeping |
| >500       | Error   | 🔴 Flashing Red | Error tone     |

## Hardware Components

### Main Components

- **STM32U083KCU6** - Ultra-low-power microcontroller
- **SGP40-D-R4** - Professional TVOC air quality sensor
- **MCP73832T** - Li-Po battery charge controller
- **ADP150AUJZ-2.5-R7** - Low-dropout voltage regulator
- **EAST1616RGBA1** - RGB LEDs (4x)
- **PKMCS0909E4000-R1** - Piezoelectric buzzer

### Power Management

- Li-Po battery charging via USB-C
- Regulated 2.5V supply for stable operation
- Ultra-low power consumption for all-day use

## 📁 What's in This Package

This ZIP file contains everything you need to build the Air Quality Monitoring Necklace Pendant with **circular casing**:

```
circular/
├── README.md                          # This file - project overview
├── Assembly-Instructions.md           # Step-by-step assembly guide (circular design)
├── Bill-of-Materials.md               # Complete component list with part numbers
├── pcb/
│   ├── pcb_schematic.pdf             # PCB schematic diagram
│   └── gerber_files.zip              # Gerber manufacturing files for PCB fabrication
├── 3d-models/
│   ├── pendant-top-circular.stl      # Top enclosure STL for 3D printing
│   └── pendant-bottom-circular.stl   # Bottom enclosure STL for 3D printing
├── firmware/
│   └── arduino_code.ino              # Arduino firmware code
└── images/
    ├── 01-pcb-assembly/               # 20 PCB assembly instruction images
    ├── 02-component-installation/     # 3 component installation images
    ├── 03-enclosure-assembly/         # 11 enclosure assembly images (circular design)
    ├── 04-testing/                    # 8 testing and verification images
    └── 05-troubleshooting/            # 8 troubleshooting guide images
```

## 🚀 Quick Start Guide

### 1. Hardware Assembly

1. **Order PCB**: Use the Gerber files in `pcb/gerber_files.zip` to order your PCB from a fabrication service
2. **3D Print Enclosure**: Use the STL files in `3d-models/` to print the circular top and bottom enclosure halves
3. **Solder Components**: Follow the detailed `Bill-of-Materials.md` and assembly instructions
4. **Assemble**: Follow the step-by-step guide in `Assembly-Instructions.md`

### 2. Software Setup

1. **Install Arduino IDE** (version 1.8.19 or newer)
2. **Add STM32 board support**
3. **Install required libraries**:
   - DFRobot_SGP40
   - PlayRtttl
   - ptScheduler
4. **Upload firmware**: Use the code in `firmware/arduino_code.ino` with ST-Link programmer

## Required Libraries

Add these libraries through Arduino IDE Library Manager:

```cpp
#include <DFRobot_SGP40.h>     // SGP40 sensor communication
#include <PlayRtttl.hpp>       // Musical tone generation
#include <ptScheduler.h>       // Non-blocking task scheduling
```

## Programming the Device

### Hardware Requirements

- **ST-Link V2 programmer** (required for STM32)
- **USB-C cable** for power and charging
- **3.3V power supply** during programming

### Upload Process

1. Connect ST-Link to SWD pins (SWDIO, SWCLK)
2. Select board: "STM32U0 series" in Arduino IDE
3. Select programmer: "STM32CubeProgrammer (SWD)"
4. Upload firmware

## PCB Specifications

- **Dimensions**: 32.5mm diameter (circular)
- **Layers**: 2-layer PCB
- **Thickness**: 1.6mm
- **Components**: SMD (0603/0402 packages)
- **Connector**: USB-C for charging

## 3D Printing Guide

### Print Settings

- **Layer Height**: 0.2mm
- **Infill**: 20%
- **Supports**: Minimal (only for overhangs)
- **Material**: PLA or PETG recommended

### Post-Processing

- Light sanding for smooth finish
- Ensure USB-C port alignment
- Test fit before final assembly

## Design Variant

This package contains files for the **Circular Casing (Original Design)** variant. The enclosure is a circular shape with a 32.5mm diameter, matching the PCB dimensions.

## Documentation Files

- **Assembly-Instructions.md**: Complete step-by-step guide with images for assembling the circular pendant
- **Bill-of-Materials.md**: Detailed component list with manufacturer part numbers, quantities, and specifications
- **README.md** (this file): Project overview and navigation guide

## Image References

All assembly images are organized in the `images/` folder:
- **PCB Assembly** (`01-pcb-assembly/`): 20 images covering component placement and soldering
- **Component Installation** (`02-component-installation/`): 3 images for battery and final component installation
- **Enclosure Assembly** (`03-enclosure-assembly/`): 11 images specific to the circular enclosure design
- **Testing** (`04-testing/`): 8 images for testing and verification procedures
- **Troubleshooting** (`05-troubleshooting/`): 8 images for common issues and solutions

## Support

- **Assembly Issues**: Refer to the troubleshooting section in `Assembly-Instructions.md`
- **Component Sourcing**: Use the part numbers in `Bill-of-Materials.md` to order from distributors (DigiKey, Mouser, Arrow, etc.)
- **PCB Fabrication**: Use `pcb/gerber_files.zip` with any PCB manufacturer

## Acknowledgments

- **CircuitDigest** - Original project development and documentation
- **DFRobot** - SGP40 sensor library
- **STMicroelectronics** - STM32 microcontroller support

---

**⭐ If this project helped you, please consider sharing your build!**

**📧 Questions?** Refer to the detailed `Assembly-Instructions.md` for step-by-step guidance.

