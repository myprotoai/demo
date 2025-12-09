# Assembly Instructions
## Air Quality Monitoring Necklace Pendant - Teardrop Casing Variant

**Project Name:** Air Quality Monitoring Necklace Pendant (Teardrop Casing - Refined Design)  
**Document Version:** 1.0  
**Date:** 2025-12-06  
**Design Variant:** Refined (Teardrop) - Generated from refined design prompt  
**Estimated Assembly Time:** 2-3 hours  
**Difficulty Level:** Intermediate (requires basic soldering skills)

---

## Table of Contents

1. [Introduction](#introduction)
2. [Safety Precautions](#safety-precautions)
3. [Required Tools and Equipment](#required-tools-and-equipment)
4. [Pre-Assembly Checklist](#pre-assembly-checklist)
5. [PCB Assembly](#pcb-assembly)
6. [Component Installation](#component-installation)
7. [Enclosure Assembly](#enclosure-assembly)
8. [Testing and Calibration](#testing-and-calibration)
9. [Troubleshooting](#troubleshooting)
10. [Final Verification](#final-verification)

---

## Introduction

This document provides step-by-step instructions for assembling the Air Quality Monitoring Necklace Pendant with **teardrop-shaped casing**. The device is a compact, wearable pendant that monitors air quality using a TVOC sensor and provides visual feedback through RGB LEDs.

### Device Overview

The pendant consists of:
- **Main PCB**: 32.5mm diameter circular board with all electronic components (unchanged from original design)
- **Enclosure**: 3D printed teardrop-shaped top and bottom halves (wider at top, tapering to pointed bottom)
- **Battery**: Rechargeable Li-Po battery (200mAh, 3.7V)
- **Necklace Chain**: Adjustable chain or cord with breakaway clasp

**Note**: The PCB remains circular (32.5mm diameter) and fits within the teardrop-shaped enclosure cavity. Only the enclosure shape has changed from the original circular design.

### Key Features

- Real-time TVOC (Total Volatile Organic Compounds) monitoring
- Color-coded LED feedback (Green/Yellow/Red)
- Audio alerts via piezoelectric buzzer
- USB-C charging capability
- All-day battery life (16+ hours)
- Elegant teardrop pendant design

---

## Safety Precautions

⚠️ **IMPORTANT: Read all safety precautions before beginning assembly**

1. **ESD Protection**: Always use an anti-static mat and wrist strap when handling components. Static electricity can damage sensitive ICs.

2. **Soldering Safety**:
   - Work in a well-ventilated area
   - Use safety glasses to protect eyes from solder splashes
   - Keep soldering iron in a secure holder when not in use
   - Allow components to cool before handling

3. **Battery Safety**:
   - Never short-circuit the battery terminals
   - Do not puncture, crush, or expose battery to extreme heat
   - Use only the specified battery type and capacity
   - Charge battery only when properly installed in device

4. **Chemical Safety**:
   - Avoid inhaling flux fumes during soldering
   - Wash hands after handling solder and flux
   - Keep cleaning solvents away from heat sources

5. **General Safety**:
   - Disconnect power before making any modifications
   - Double-check component orientation before soldering
   - Verify polarity of all polarized components

---

## Required Tools and Equipment

### Essential Tools

| Tool | Specification | Purpose |
|------|---------------|---------|
| Soldering Iron | 30-40W, adjustable temperature (300-400°C) | Component soldering |
| Solder | Lead-free, 0.5-0.8mm diameter, rosin core | Electrical connections |
| Solder Wick | 2-3mm width | Desoldering and cleanup |
| Flux | Rosin-based, no-clean | Improved solder flow |
| Tweezers | ESD-safe, fine tip | Component placement |
| Wire Cutters | Flush cut | Lead trimming |
| Multimeter | Digital, basic functions | Continuity and voltage testing |
| Magnifying Glass | 3-5x magnification | Inspection of small components |
| Anti-static Mat | ESD-safe workspace | Static protection |
| Anti-static Wrist Strap | ESD-safe | Personal static protection |

### Optional but Recommended

- Hot air rework station (for SMD components)
- Solder paste stencil (for batch assembly)
- Component organizer trays
- Helping hands tool
- Isopropyl alcohol and lint-free wipes (for cleaning)

### Software Tools

- ST-Link V2 programmer (for firmware upload)
- USB-C cable (for charging and programming)
- Arduino IDE or STM32CubeIDE (for firmware development)

---

## Pre-Assembly Checklist

Before beginning assembly, verify you have all required components:

### Component Verification

- [ ] PCB received and inspected for damage
- [ ] All components from BOM verified and organized
- [ ] 3D printed teardrop enclosure parts received (top and bottom halves)
- [ ] Battery received and checked for damage
- [ ] Necklace chain/cord received
- [ ] All tools available and in working condition

### Workspace Setup

- [ ] Clean, well-lit workspace prepared
- [ ] Anti-static mat laid out
- [ ] Anti-static wrist strap ready
- [ ] Soldering station set up and tested
- [ ] Component organizer trays labeled
- [ ] Safety equipment (glasses, ventilation) ready

### PCB Inspection

1. **Visual Inspection**:
   - Check PCB for scratches, cracks, or delamination
   - Verify all pads are clean and free of oxidation
   - Check for any manufacturing defects
   - Verify silkscreen labels are clear and readable

2. **Continuity Check**:
   - Use multimeter to verify no short circuits between power and ground
   - Check for any obvious manufacturing errors

---

## PCB Assembly

**Note**: The PCB assembly process is identical to the original circular design since the PCB itself remains circular (32.5mm diameter). The PCB fits within the teardrop-shaped enclosure cavity.

### Step 1: Prepare Workspace

![PCB Overview](assembly-images/01-pcb-assembly/01-pcb-overview.png)

1. Put on anti-static wrist strap and connect to ground
2. Place PCB on anti-static mat
3. Organize components by package size for easy access
4. Set soldering iron to appropriate temperature (350°C for lead-free solder)

**Reference**: See PCB overview image above for component locations.

### Step 2: Install Passive Components (Resistors and Capacitors)

![Component Placement Map](assembly-images/01-pcb-assembly/02-component-placement-map.png)

**Order of Installation**: Start with smallest components and work up to larger ones. Follow the color-coded installation sequence shown in the component placement map above.

#### 2.1 Install Resistors (R1-R5)

![Resistor Installation](assembly-images/01-pcb-assembly/03-resistor-installation.png)

1. **R1 (10kΩ)**:
   - Locate R1 position on PCB (check silkscreen)
   - Verify resistor value using multimeter (should read ~10kΩ)
   - Place resistor on PCB pads
   - Verify orientation (resistors are non-polarized)
   - Solder one pad, check alignment, then solder second pad
   - Trim excess leads flush to board

2. **R2 (4.7kΩ)**:
   - Repeat process for R2
   - Verify value: ~4.7kΩ

3. **R3 (2.2kΩ)**:
   - Repeat process for R3
   - Verify value: ~2.2kΩ

4. **R4 (100Ω, 4x)**:
   - Install all four R4 resistors
   - Verify value: ~100Ω each

5. **R5 (220Ω, 4x)**:
   - Install all four R5 resistors
   - Verify value: ~220Ω each

**Verification**: Use multimeter to check each resistor value after installation.

#### 2.2 Install Capacitors (C1-C7)

![Capacitor Installation](assembly-images/01-pcb-assembly/04-capacitor-installation.png)

1. **C1, C2 (10µF)**:
   - Locate C1 and C2 positions
   - **IMPORTANT**: Ceramic capacitors are non-polarized
   - Place capacitors on pads
   - Solder both pads
   - Trim excess leads

2. **C3 (4.7µF)**:
   - Install C3 using same process

3. **C4-C7 (100nF, 4x)**:
   - Install all four 100nF capacitors
   - These are decoupling capacitors - ensure they're close to their respective ICs

**Verification**: Check for proper solder joints and no bridges between pads.

### Step 3: Install Power Management Components

#### 3.1 Install Voltage Regulator (U4 - ADP150)

![Voltage Regulator Installation](assembly-images/01-pcb-assembly/05-voltage-regulator-installation.png)

1. **Identify Pin 1**:
   - Locate pin 1 indicator on IC (usually a dot or notch)
   - Match with pin 1 indicator on PCB silkscreen

2. **Placement**:
   - Apply small amount of flux to pads
   - Place IC on pads, ensuring pin 1 alignment
   - Verify all pins are on their respective pads

3. **Soldering**:
   - For TSOT-23 package, use fine-tip soldering iron
   - Solder pin 1 first to secure position
   - Solder remaining pins carefully
   - Check for solder bridges between pins
   - Use solder wick to remove any bridges

**Verification**: 
- Check continuity between pins and pads
- Verify no short circuits between adjacent pins

#### 3.2 Install Battery Charge Controller (U3 - MCP73832)

![Charge Controller Installation](assembly-images/01-pcb-assembly/06-charge-controller-installation.png)

1. Follow same process as U4
2. **Critical**: Ensure correct orientation (pin 1 to pin 1)
3. This IC manages battery charging - incorrect installation will prevent charging

**Verification**: Check pin alignment and solder quality.

#### 3.3 Install Schottky Diode (D1)

**Note**: Diode orientation is critical. Match the cathode stripe (marked on diode) with the silkscreen marking on PCB.

1. **Identify Cathode**:
   - Diode has a stripe on cathode end
   - Match cathode stripe with silkscreen marking on PCB

2. **Placement and Soldering**:
   - Place diode with correct orientation
   - Solder both pads
   - **WARNING**: Reversed polarity will damage circuit

**Verification**: Check orientation matches silkscreen.

### Step 4: Install Microcontroller (U1 - STM32U083KCU6)

⚠️ **CRITICAL STEP**: This is the most important component. Take extra care.

![Microcontroller Overview](assembly-images/01-pcb-assembly/07-microcontroller-overview.png)

1. **Preparation**:
   - Verify microcontroller part number matches BOM
   - Check for any bent pins
   - Clean pads on PCB with isopropyl alcohol

2. **Pin 1 Identification**:
   - Locate pin 1 indicator on IC (usually a dot in corner)
   - Match with pin 1 indicator on PCB (usually a square pad or dot)

![Pin 1 Alignment](assembly-images/01-pcb-assembly/08-microcontroller-pin1-alignment.png)

3. **Placement**:
   - For QFN-48 package, alignment is critical
   - Apply flux to PCB pads
   - Carefully place IC, ensuring pin 1 alignment
   - Verify all pads are visible around IC perimeter

4. **Soldering**:
   - **Method 1 (Hot Air)**:
     - Use hot air rework station
     - Apply heat evenly around IC (350°C, low airflow)
     - Watch for solder to flow and IC to "settle"
     - Allow to cool before moving
   
   - **Method 2 (Soldering Iron)**:
     - Solder corner pins first to secure position
     - Apply flux to all pads
     - Drag solder technique: apply solder to iron tip, drag across pins
     - Use solder wick to remove excess and bridges
     - Check each pin for proper connection

![Soldering Methods](assembly-images/01-pcb-assembly/09-microcontroller-soldering-methods.png)

5. **Verification**:
   - Inspect all pins under magnification
   - Check for solder bridges
   - Verify no cold solder joints
   - Test continuity between adjacent pins (should be open circuit)

![Microcontroller Verification](assembly-images/01-pcb-assembly/10-microcontroller-verification.png)

### Step 5: Install Air Quality Sensor (U2 - SGP40)

![Sensor Installation](assembly-images/01-pcb-assembly/11-sensor-installation.png)

1. **Sensor Orientation**:
   - SGP40 has air sampling vents on top
   - Ensure vents face upward (away from PCB) when installed
   - Match pin 1 with PCB pin 1 indicator

2. **Placement**:
   - Apply thermal pad to sensor bottom (if specified)
   - Place sensor on PCB pads
   - Verify air vents are not blocked

3. **Soldering**:
   - Use fine-tip soldering iron
   - Solder all 8 pins carefully
   - **IMPORTANT**: Do not overheat sensor - it contains sensitive sensing elements

4. **Air Vent Clearance**:
   - Verify sensor vents have clearance above PCB
   - Ensure teardrop enclosure will not block air flow to sensor

**Verification**: 
- Check sensor is properly seated
- Verify air vents are accessible
- Test I2C communication (requires firmware)

### Step 6: Install RGB LEDs (LED1-LED4)

![LED Installation Overview](assembly-images/01-pcb-assembly/12-led-installation-overview.png)

1. **LED Identification**:
   - EAST1616RGBA1 LEDs have 4 pins (R, G, B, Common Anode)
   - Identify pin 1 (usually marked with dot or different pad shape)
   - Match with PCB silkscreen

2. **Installation Process** (repeat for all 4 LEDs):
   - Place LED on PCB pads
   - Verify pin 1 alignment
   - Solder all 4 pins
   - **IMPORTANT**: LEDs are directional - incorrect orientation will prevent operation

![LED Installation Detail](assembly-images/01-pcb-assembly/13-led-installation-detail.png)

3. **LED Placement**:
   - LEDs should be positioned to maximize visibility through teardrop enclosure openings
   - Ensure LEDs are flush with PCB surface
   - Check that LED lenses are not scratched

**Verification**: 
- Visual inspection of all LED installations
- Verify pin alignment matches silkscreen
- Test LEDs after power-up (requires firmware)

### Step 7: Install Piezoelectric Buzzer (BZ1)

![Buzzer Installation](assembly-images/01-pcb-assembly/14-buzzer-installation.png)

1. **Buzzer Orientation**:
   - Piezoelectric buzzers are polarized
   - Identify positive (+) and negative (-) terminals
   - Match with PCB markings

2. **Placement**:
   - Place buzzer on PCB pads
   - Ensure correct polarity
   - Buzzer should be positioned to allow sound to escape teardrop enclosure

3. **Soldering**:
   - Solder both terminals
   - Verify secure mechanical connection

**Verification**: Check polarity and secure mounting.

### Step 8: Install Crystal Oscillator (Y1)

**Note**: Crystals are non-polarized. Place on PCB pads and solder both terminals.

1. **Crystal Installation**:
   - Crystals are non-polarized
   - Place crystal on PCB pads
   - Solder both terminals
   - Keep leads as short as possible

2. **Mounting Considerations**:
   - Crystal should be close to microcontroller
   - Avoid mechanical stress on crystal

**Verification**: Check solder joints and positioning.

### Step 9: Install Connectors

#### 9.1 USB Type-C Connector (J1)

![USB-C Connector Installation](assembly-images/01-pcb-assembly/15-usbc-connector-installation.png)

1. **Connector Orientation**:
   - USB-C connectors have specific mounting orientation
   - Match connector keying with PCB cutout
   - Verify connector will align with teardrop enclosure side opening

2. **Placement and Soldering**:
   - Insert connector into PCB from top side
   - Solder all pins (USB-C has many pins - be thorough)
   - Verify connector is flush with PCB surface
   - Check for proper mechanical retention

**Verification**: 
- Verify connector alignment with teardrop enclosure side opening
- Test connector retention (should not wobble)

#### 9.2 Battery Connector (J2)

![Battery Connector Installation](assembly-images/01-pcb-assembly/16-battery-connector-installation.png)

1. **Connector Type**:
   - JST PH 2-pin connector
   - Identify positive and negative terminals
   - Match with PCB markings (+ and -)

2. **Installation**:
   - Insert connector from bottom of PCB
   - Solder both pins
   - **CRITICAL**: Verify polarity - reversed connection will damage battery and circuit

**Verification**: Double-check polarity before connecting battery.

#### 9.3 SWD Programming Header (P1)

![Programming Header Installation](assembly-images/01-pcb-assembly/17-programming-header-installation.png)

1. **Header Installation**:
   - 4-pin header for ST-Link programming
   - Insert header from bottom of PCB
   - Solder all 4 pins
   - Header pins should extend below PCB for programming access

2. **Pin Configuration** (for reference):
   - Pin 1: VDD (3.3V)
   - Pin 2: SWDIO
   - Pin 3: SWCLK
   - Pin 4: GND

**Verification**: Check pin alignment and solder quality.

### Step 10: PCB Assembly Verification

![Complete PCB Top View](assembly-images/01-pcb-assembly/18-complete-pcb-top-view.png)

![Complete PCB Bottom View](assembly-images/01-pcb-assembly/19-complete-pcb-bottom-view.png)

1. **Visual Inspection**:
   - Check all components are installed
   - Verify component orientations
   - Look for solder bridges
   - Check for cold solder joints
   - Verify no components are damaged

2. **Continuity Testing**:
   - Test power rails (VDD to GND should not be shorted)
   - Verify I2C bus connections (SDA, SCL)
   - Check USB-C connector pins
   - Test battery connector polarity

3. **Component Verification**:
   - Verify all resistors and capacitors are installed
   - Check all ICs are properly oriented
   - Confirm LEDs are correctly placed
   - Verify sensor is properly mounted

![PCB Verification Checklist](assembly-images/01-pcb-assembly/20-pcb-verification-checklist.png)

---

## Component Installation

### Step 11: Battery Installation

⚠️ **BATTERY SAFETY**: Handle battery with care. Never short-circuit terminals.

![Battery Mounting](assembly-images/02-component-installation/22-battery-mounting.png)

1. **Battery Preparation**:
   - Verify battery specifications match BOM (3.7V, 200mAh minimum)
   - Check battery for any physical damage
   - Verify battery protection circuit is present

2. **Battery Mounting**:
   - Apply double-sided adhesive to battery back
   - Position battery in bottom teardrop enclosure half
   - Ensure battery does not interfere with PCB placement
   - Route battery wires to connector location

3. **Battery Connection**:
   - **DO NOT CONNECT YET** - wait until final assembly
   - Verify connector polarity matches battery wires
   - Red wire = Positive (+)
   - Black wire = Negative (-)

![Battery Connection Detail](assembly-images/02-component-installation/23-battery-connection-detail.png)

**Verification**: 
- Battery fits securely in teardrop enclosure
- Wires are long enough to reach connector
- Polarity is clearly marked

---

## Enclosure Assembly

### Step 12: Prepare Teardrop Enclosure Parts

![Enclosure Parts Overview - Teardrop](assembly-images/03-enclosure-assembly/31-enclosure-parts-overview-teardrop.png)

1. **Inspect 3D Printed Teardrop Parts**:
   - Check top and bottom teardrop halves for defects
   - Verify teardrop shape: wider at top (35-40mm), tapering to pointed bottom (15-20mm)
   - Verify all mounting holes are clear
   - Check USB-C opening alignment on side wall (near top, wider section)
   - Ensure sensor air vent openings are present
   - Verify side slots (2x, horizontal oval, near top) are present
   - Check attachment loop at top center
   - Lightly sand any rough surfaces, especially curved areas

![Enclosure Preparation - Teardrop](assembly-images/03-enclosure-assembly/32-enclosure-preparation-teardrop.png)

2. **Test Fit Circular PCB in Teardrop Enclosure**:
   - Place circular PCB (32.5mm diameter) in bottom teardrop enclosure
   - Verify PCB fits within teardrop cavity without forcing
   - Check minimum 1-2mm clearance on all sides
   - Verify USB-C connector aligns with side opening
   - Ensure sensor vents align with enclosure openings
   - Verify LEDs are visible through enclosure openings
   - Check that PCB does not interfere with teardrop shape

### Step 13: Install PCB into Teardrop Enclosure

![PCB Placement - Teardrop](assembly-images/03-enclosure-assembly/33-pcb-placement-teardrop.png)

1. **Place PCB**:
   - Position circular PCB in bottom teardrop enclosure half
   - Align mounting holes with enclosure posts
   - Verify PCB fits within teardrop cavity (circular PCB in teardrop shape)
   - Verify USB-C connector protrudes through side opening
   - Check sensor is properly positioned
   - Ensure 1-2mm clearance on all sides

2. **Install Spacers**:
   - Place M1.6 spacers on mounting posts
   - Spacers provide clearance between PCB and teardrop enclosure

![Spacer Installation - Teardrop](assembly-images/03-enclosure-assembly/34-spacer-installation-teardrop.png)

3. **Secure PCB**:
   - Use M1.6x4 screws to secure PCB
   - Tighten screws gently - do not overtighten (may crack 3D printed parts)
   - Verify PCB is secure but not stressed

![PCB Securing - Teardrop](assembly-images/03-enclosure-assembly/35-pcb-securing-teardrop.png)

**Verification**: 
- PCB is securely mounted within teardrop enclosure
- All connectors align with openings
- No components are touching teardrop enclosure walls
- Circular PCB fits properly in teardrop cavity

### Step 14: Connect Battery

⚠️ **FINAL CHECK BEFORE CONNECTING**:

![Pre-Connection Verification - Teardrop](assembly-images/03-enclosure-assembly/36-pre-connection-verification-teardrop.png)
- [ ] All components verified
- [ ] No short circuits detected
- [ ] Battery polarity confirmed
- [ ] Connector orientation verified

1. **Connect Battery**:
   - Align battery connector with PCB connector
   - Verify polarity one more time
   - Gently push connectors together
   - Listen for click indicating secure connection

![Battery Connection Final - Teardrop](assembly-images/03-enclosure-assembly/37-battery-connection-final-teardrop.png)

2. **Initial Power Test**:
   - Device should power on (if firmware is loaded)
   - LEDs may light up
   - Check for any unusual behavior
   - If smoke or heat detected, disconnect immediately

**Verification**: Device powers on without issues.

### Step 15: Close Teardrop Enclosure

1. **Final Inspection**:
   - Verify all components are properly positioned
   - Check battery wires are not pinched
   - Ensure sensor vents are clear
   - Verify USB-C connector is accessible through side opening
   - Check that circular PCB fits properly within teardrop cavity

2. **Align Teardrop Enclosure Halves**:
   - Place top teardrop enclosure half over bottom
   - Align mounting holes
   - Verify teardrop shapes match perfectly
   - Check attachment loops align at top
   - Verify side slots align
   - Ensure sensor vents align

![Enclosure Closure Alignment - Teardrop](assembly-images/03-enclosure-assembly/38-enclosure-closure-alignment-teardrop.png)

3. **Secure Enclosure**:
   - Use remaining M1.6x4 screws
   - Tighten evenly in cross pattern
   - Do not over-tighten - may crack 3D printed teardrop parts

![Enclosure Closure Securing - Teardrop](assembly-images/03-enclosure-assembly/39-enclosure-closure-securing-teardrop.png)

4. **Final Check**:
   - Verify teardrop enclosure is secure
   - Check all openings are clear (USB-C, sensor vents, side slots)
   - Ensure device can be charged via USB-C
   - Verify teardrop shape is maintained

### Step 16: Attach Necklace Chain

![Chain Attachment - Teardrop](assembly-images/03-enclosure-assembly/310-chain-attachment-teardrop.png)

1. **Chain Attachment**:
   - Thread chain through attachment loop at top of teardrop pendant (wider end)
   - Use breakaway clasp for safety
   - Adjust chain length as desired

2. **Final Assembly Check**:
   - Verify pendant hangs properly with teardrop shape
   - Check chain does not interfere with USB-C port on side
   - Ensure device is comfortable to wear
   - Verify teardrop shape is aesthetically pleasing

![Complete Assembly External - Teardrop](assembly-images/03-enclosure-assembly/311-complete-assembly-external-teardrop.png)

---

## Testing and Calibration

### Step 17: Power-On Test

![Power-On Test Setup - Teardrop](assembly-images/04-testing/41-power-on-test-setup-teardrop.png)

1. **Initial Power Test**:
   - Connect USB-C cable to charger
   - Plug into power source
   - Observe device behavior:
     - LEDs should indicate charging status
     - No smoke or unusual heat
     - No error beeps

2. **Voltage Verification** (if multimeter available):
   - Measure voltage at battery connector (should be ~3.7V)
   - Check regulator output (should be 2.5V)
   - Verify no short circuits

### Step 18: Firmware Upload

![ST-Link Connection - Teardrop](assembly-images/04-testing/42-stlink-connection-teardrop.png)

1. **Connect ST-Link**:
   - Connect ST-Link V2 to SWD header (P1)
   - Verify connections:
     - VDD to VDD
     - SWDIO to SWDIO
     - SWCLK to SWCLK
     - GND to GND

2. **Upload Firmware**:
   - Open Arduino IDE or STM32CubeIDE
   - Select board: STM32U0 series
   - Select programmer: ST-Link
   - Upload firmware
   - Verify successful upload

![Firmware Upload - Teardrop](assembly-images/04-testing/43-firmware-upload-teardrop.png)

3. **Disconnect ST-Link**:
   - Safely disconnect programming cable
   - Device should now run firmware

### Step 19: Functional Testing

1. **LED Test**:
   - Device should display color based on air quality
   - Green = Good air (TVOC 0-200)
   - Yellow = Moderate air (TVOC 201-300)
   - Red = Poor air (TVOC 301-500)
   - Test by exposing sensor to different air conditions
   - Verify LEDs are visible through teardrop enclosure openings

![LED Color Test - Teardrop](assembly-images/04-testing/44-led-color-test-teardrop.png)

2. **Sensor Test**:
   - Wave hand near sensor (should detect changes)
   - Test in different environments (indoor, outdoor)
   - Verify sensor responds to air quality changes
   - Ensure sensor vents in teardrop enclosure allow proper air flow

![Sensor Response Test - Teardrop](assembly-images/04-testing/45-sensor-response-test-teardrop.png)

3. **Audio Test**:
   - Verify buzzer sounds for alerts
   - Test different alert tones
   - Check volume is appropriate
   - Ensure sound escapes through teardrop enclosure

![Audio Test - Teardrop](assembly-images/04-testing/46-audio-test-teardrop.png)

4. **Battery Test**:
   - Charge battery fully
   - Monitor battery life over time
   - Verify 16+ hour operation

![Battery Life Test - Teardrop](assembly-images/04-testing/47-battery-life-test-teardrop.png)

5. **Charging Test**:
   - Connect USB-C charger through side opening
   - Verify charging indicator
   - Test charging completes successfully

![Charging Test - Teardrop](assembly-images/04-testing/48-charging-test-teardrop.png)

### Step 20: Calibration (if required)

1. **Sensor Calibration**:
   - Some sensors may require baseline calibration
   - Follow firmware instructions for calibration
   - Calibrate in clean air environment

2. **LED Calibration**:
   - Verify color accuracy
   - Adjust if necessary (via firmware)

---

## Troubleshooting

### Common Issues and Solutions

#### Issue 1: Device Does Not Power On

**Symptoms**: No LEDs, no response when USB connected

![Short Circuit Detection - Teardrop](assembly-images/05-troubleshooting/51-short-circuit-detection-teardrop.png)

**Possible Causes**:
- Battery not connected or incorrectly connected
- Short circuit on PCB
- Faulty power management IC

**Solutions**:
1. Check battery connection and polarity
2. Verify no short circuits with multimeter
3. Check U3 and U4 are properly installed
4. Verify battery voltage (should be 3.7V)

#### Issue 2: LEDs Do Not Light

**Symptoms**: Device powers on but LEDs remain off

![LED Not Working - Teardrop](assembly-images/05-troubleshooting/58-led-not-working-teardrop.png)

**Possible Causes**:
- LEDs installed with incorrect polarity
- Faulty LED connections
- Firmware issue
- LEDs not visible through teardrop enclosure openings

**Solutions**:
1. Verify LED polarity matches PCB markings
2. Check LED solder joints
3. Test LEDs individually with multimeter
4. Verify firmware is correctly uploaded
5. Check that LEDs align with teardrop enclosure openings

![Orientation Errors - Teardrop](assembly-images/05-troubleshooting/52-orientation-errors-teardrop.png)

#### Issue 3: Sensor Not Responding

**Symptoms**: LEDs show same color regardless of air quality

![Sensor Vent Blockage - Teardrop](assembly-images/05-troubleshooting/55-sensor-vent-blockage-teardrop.png)

**Possible Causes**:
- Sensor not properly connected
- I2C communication issue
- Sensor blocked or damaged
- Sensor vents blocked by teardrop enclosure

**Solutions**:
1. Verify sensor is properly soldered
2. Check I2C bus connections (SDA, SCL)
3. Ensure sensor vents are not blocked by teardrop enclosure
4. Verify air flow path through teardrop enclosure openings
5. Test sensor with multimeter (check power pins)

#### Issue 4: Battery Not Charging

**Symptoms**: Device works but battery does not charge via USB

![USB-C Connection Issues - Teardrop](assembly-images/05-troubleshooting/56-usbc-connection-issues-teardrop.png)

**Possible Causes**:
- USB-C connector not properly installed
- Charge controller (U3) issue
- Battery protection circuit triggered
- USB-C connector not accessible through teardrop enclosure side opening

**Solutions**:
1. Verify USB-C connector is properly soldered
2. Check U3 installation and orientation
3. Test USB-C connection with multimeter
4. Verify USB-C connector aligns with teardrop enclosure side opening
5. Verify battery protection circuit is functioning

![Battery Connection Problems - Teardrop](assembly-images/05-troubleshooting/57-battery-connection-problems-teardrop.png)

#### Issue 5: Device Overheats

**Symptoms**: Device becomes hot during operation

**Possible Causes**:
- Short circuit
- Faulty component
- Overcurrent condition

**Solutions**:
1. **IMMEDIATELY DISCONNECT POWER**
2. Check for short circuits
3. Verify all components are correct values
4. Check for damaged components

#### Issue 6: Teardrop Enclosure Does Not Close Properly

**Symptoms**: Teardrop enclosure halves do not fit together

**Possible Causes**:
- Components too tall
- PCB not properly seated in teardrop cavity
- Enclosure printing defects
- Circular PCB not fitting properly in teardrop shape

**Solutions**:
1. Verify all components are properly seated on PCB
2. Check PCB mounting and spacer height
3. Verify circular PCB fits within teardrop cavity (1-2mm clearance)
4. Verify 3D printed teardrop parts match specifications
5. Lightly sand teardrop enclosure if needed, especially curved areas

---

## Final Verification

### Step 21: Complete System Check

Perform final verification:

- [ ] Device powers on successfully
- [ ] LEDs display correct colors for air quality
- [ ] Sensor responds to air quality changes
- [ ] Audio alerts function properly
- [ ] Battery charges via USB-C through side opening
- [ ] Battery provides 16+ hours of operation
- [ ] Teardrop enclosure is secure and properly closed
- [ ] All openings (USB-C, sensor vents, side slots) are clear
- [ ] Necklace chain is properly attached at top
- [ ] Device is comfortable to wear
- [ ] Teardrop shape is aesthetically pleasing
- [ ] No unusual heat or behavior
- [ ] Firmware functions as expected

### Step 22: Documentation

1. **Record Serial Number** (if applicable)
2. **Note Any Modifications** made during assembly
3. **Document Calibration Values** (if calibrated)
4. **Keep Assembly Notes** for future reference

---

## Maintenance and Care

### Regular Maintenance

1. **Cleaning**:
   - Clean sensor vents periodically (ensure teardrop enclosure vents are clear)
   - Wipe teardrop enclosure with soft cloth
   - Avoid harsh chemicals

2. **Battery Care**:
   - Charge battery regularly
   - Avoid complete discharge
   - Store in cool, dry place

3. **Inspection**:
   - Periodically check for damage
   - Verify all functions still work
   - Check battery health
   - Inspect teardrop enclosure for cracks or wear

### Storage

- Store device in protective case
- Keep battery charged (50-80% for long-term storage)
- Avoid extreme temperatures
- Protect from moisture

---

## Support and Resources

### Additional Resources

- **Schematic Diagrams**: Available in project repository
- **Firmware Code**: Available in project repository
- **3D Model Files**: STL files for teardrop enclosure printing
- **Community Forums**: [Link to project discussion forum]

### Getting Help

If you encounter issues not covered in this guide:

1. Check troubleshooting section
2. Review schematic and PCB layout
3. Consult project documentation
4. Post questions in project forum
5. Contact project maintainers

---

## Appendix

### A. Component Datasheets

Key component datasheets for reference:
- STM32U083KCU6: [STMicroelectronics website]
- SGP40: [Sensirion website]
- MCP73832: [Microchip website]
- ADP150: [Analog Devices website]

### B. Tool Recommendations

Recommended tools for best results:
- Hakko FX-888D soldering station
- Weller WES51 (alternative)
- Kester 44 rosin core solder
- Chemtronics solder wick

### C. Additional Notes

- Assembly time may vary based on experience level
- First-time builders should allow extra time
- Practice soldering on scrap PCB if new to SMD work
- Take breaks to avoid fatigue and mistakes
- **Teardrop Enclosure Note**: The circular PCB (32.5mm diameter) fits within the teardrop-shaped enclosure cavity. Ensure proper clearance (1-2mm minimum) on all sides when placing PCB in teardrop enclosure.

---

**Document Control:**
- Prepared by: ProtoAI Design System
- Reviewed by: [To be assigned]
- Approved by: [To be assigned]
- Next Review Date: [To be determined]

**Revision History:**
- v1.0 (2025-12-06): Initial release - Teardrop Casing Variant

---

**End of Assembly Instructions**

