# Bill of Materials (BOM)
## Air Quality Monitoring Necklace Pendant

**Project Name:** Air Quality Monitoring Necklace Pendant  
**Document Version:** 1.0  
**Date:** 2025-12-06  
**PCB Revision:** Rev 1.0

---

## Active Components

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| U1 | 1 | STM32U083KCU6 | Ultra-low-power 32-bit ARM Cortex-M33 MCU | QFN-48 | 32-bit, 48MHz, 256KB Flash, 32KB RAM | STMicroelectronics | Microcontroller |
| U2 | 1 | SGP40-D-R4 | TVOC Air Quality Sensor | DFN-8 | I2C Interface, 0-60000 ppb range | Sensirion | Sensor |
| U3 | 1 | MCP73832T-2ACI/OT | Li-Po Battery Charge Controller | SOT-23-5 | 4.2V, 500mA max charge current | Microchip Technology | Power Management |
| U4 | 1 | ADP150AUJZ-2.5-R7 | Low-Dropout Voltage Regulator | TSOT-23-5 | 2.5V, 150mA output | Analog Devices | Power Management |

## LEDs and Indicators

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| LED1 | 1 | EAST1616RGBA1 | RGB LED | 1.6x1.6mm | Red/Green/Blue, Common Anode | Everlight Electronics | LED |
| LED2 | 1 | EAST1616RGBA1 | RGB LED | 1.6x1.6mm | Red/Green/Blue, Common Anode | Everlight Electronics | LED |
| LED3 | 1 | EAST1616RGBA1 | RGB LED | 1.6x1.6mm | Red/Green/Blue, Common Anode | Everlight Electronics | LED |
| LED4 | 1 | EAST1616RGBA1 | RGB LED | 1.6x1.6mm | Red/Green/Blue, Common Anode | Everlight Electronics | LED |

## Audio Components

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| BZ1 | 1 | PKMCS0909E4000-R1 | Piezoelectric Buzzer | 9x9mm | 4kHz, 85dB @ 10cm | Murata Manufacturing | Audio |

## Passive Components - Resistors

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| R1 | 1 | RC0603FR-0710KL | Resistor | 0603 | 10kΩ, ±1%, 1/10W | Yageo | Resistor |
| R2 | 1 | RC0603FR-074K7L | Resistor | 0603 | 4.7kΩ, ±1%, 1/10W | Yageo | Resistor |
| R3 | 1 | RC0603FR-072K2L | Resistor | 0603 | 2.2kΩ, ±1%, 1/10W | Yageo | Resistor |
| R4 | 4 | RC0603FR-07100RL | Resistor | 0603 | 100Ω, ±1%, 1/10W | Yageo | Resistor |
| R5 | 4 | RC0603FR-07220RL | Resistor | 0603 | 220Ω, ±1%, 1/10W | Yageo | Resistor |

## Passive Components - Capacitors

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| C1 | 1 | CL10A106MQ8NRNC | Ceramic Capacitor | 0805 | 10µF, 25V, X7R | Samsung Electro-Mechanics | Capacitor |
| C2 | 1 | CL10A106MQ8NRNC | Ceramic Capacitor | 0805 | 10µF, 25V, X7R | Samsung Electro-Mechanics | Capacitor |
| C3 | 1 | CL10A475MQ8NRNC | Ceramic Capacitor | 0805 | 4.7µF, 25V, X7R | Samsung Electro-Mechanics | Capacitor |
| C4 | 1 | CL10A104KA8NNNC | Ceramic Capacitor | 0603 | 100nF, 50V, X7R | Samsung Electro-Mechanics | Capacitor |
| C5 | 1 | CL10A104KA8NNNC | Ceramic Capacitor | 0603 | 100nF, 50V, X7R | Samsung Electro-Mechanics | Capacitor |
| C6 | 1 | CL10A104KA8NNNC | Ceramic Capacitor | 0603 | 100nF, 50V, X7R | Samsung Electro-Mechanics | Capacitor |
| C7 | 1 | CL10A104KA8NNNC | Ceramic Capacitor | 0603 | 100nF, 50V, X7R | Samsung Electro-Mechanics | Capacitor |

## Connectors and Interfaces

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| J1 | 1 | USB-C-31-M-12 | USB Type-C Connector | Through-hole | USB 2.0, Power/Data | CUI Devices | Connector |
| J2 | 1 | 51021-0200 | Battery Connector | Through-hole | 2-pin JST PH connector | Molex | Connector |
| P1 | 1 | 200-10-104-00-001101 | SWD Programming Header | Through-hole | 4-pin 2.54mm pitch | Preci-Dip | Connector |

## Power Components

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| BAT1 | 1 | LP402025 | Lithium Polymer Battery | Custom | 3.7V, 200mAh, 25x20x4mm | Generic | Battery |
| D1 | 1 | BAT54C | Schottky Diode | SOT-23 | 30V, 200mA | Nexperia | Diode |

## Crystals and Oscillators

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| Y1 | 1 | ABM8G-32.000MHZ-4Y-T3 | Crystal Oscillator | 3.2x2.5mm | 32MHz, ±20ppm | Abracon | Crystal |

## PCB and Hardware

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| PCB1 | 1 | Custom | Printed Circuit Board | 32.5mm diameter | 2-layer, 1.6mm thickness, ENIG finish | Custom Fabrication | PCB |
| SCREW1 | 4 | M1.6x4 | Enclosure Screw | M1.6 | 4mm length, Phillips head | Generic | Hardware |
| SPACER1 | 4 | M1.6x3 | PCB Spacer | M1.6 | 3mm height, threaded | Generic | Hardware |

## Enclosure Components

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| ENC1 | 1 | Custom 3D Printed | Pendant Top Enclosure | STL | PLA/PETG, 0.2mm layer height | 3D Printing | Enclosure |
| ENC2 | 1 | Custom 3D Printed | Pendant Bottom Enclosure | STL | PLA/PETG, 0.2mm layer height | 3D Printing | Enclosure |
| CHAIN1 | 1 | Custom | Necklace Chain/Cord | Custom | Adjustable length, breakaway clasp | Generic | Enclosure |

## Miscellaneous

| Ref | Qty | Manufacturer Part Number | Component Name | Package | Value/Specification | Manufacturer | Category |
|-----|-----|--------------------------|----------------|---------|---------------------|--------------|----------|
| - | 1 | - | Thermal Pad | Custom | 0.5mm thickness, for sensor mounting | Generic | Thermal Management |
| - | 1 | - | Double-sided Adhesive | Custom | 0.1mm thickness, for battery mounting | Generic | Adhesive |

---

## Component Summary by Category

| Category | Total Quantity |
|----------|---------------|
| Microcontroller | 1 |
| Sensors | 1 |
| Power Management ICs | 2 |
| LEDs | 4 |
| Audio Components | 1 |
| Resistors | 9 |
| Capacitors | 7 |
| Connectors | 3 |
| Battery | 1 |
| Diodes | 1 |
| Crystals | 1 |
| PCB | 1 |
| Hardware (Screws/Spacers) | 8 |
| Enclosure Parts | 3 |
| Miscellaneous | 2 |

**Total Component Count:** 45 unique components  
**Total Part Count:** 49 parts (including multiples)

---

## Notes

1. **Component Sourcing**: All components listed use industry-standard part numbers and are available through major distributors (DigiKey, Mouser, Arrow, etc.)

2. **PCB Specifications**: 
   - 2-layer PCB design
   - 32.5mm diameter circular board
   - 1.6mm board thickness
   - ENIG (Electroless Nickel Immersion Gold) surface finish
   - Minimum trace width: 0.1mm
   - Minimum via size: 0.2mm

3. **Battery Specifications**:
   - Lithium Polymer (Li-Po) battery
   - Nominal voltage: 3.7V
   - Capacity: 200mAh minimum
   - Dimensions: 25mm x 20mm x 4mm (or similar compact form factor)
   - Must include built-in protection circuit

4. **Enclosure Specifications**:
   - 3D printed from PLA or PETG material
   - Layer height: 0.2mm recommended
   - Infill: 20% minimum
   - Post-processing: Light sanding for smooth finish
   - Must provide ventilation for sensor air sampling

5. **Assembly Considerations**:
   - All SMD components are hand-solderable with appropriate tools
   - Use lead-free solder (RoHS compliant)
   - Follow ESD precautions during assembly
   - Verify component orientation before soldering

6. **Regulatory Compliance**:
   - Components should be RoHS compliant
   - Battery must meet UN38.3 transportation requirements
   - Consider CE/FCC compliance for final product

---

**Document Control:**
- Prepared by: ProtoAI Design System
- Reviewed by: [To be assigned]
- Approved by: [To be assigned]
- Next Review Date: [To be determined]

