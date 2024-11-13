# QFHBAL01 - Antenna Interface and Balun

The **QFHBAL01** module is an [antenna interface and balun](https://en.wikipedia.org/wiki/Balun) designed for QFH (Quadrifilar Helix) antennas, supporting right-hand (RHCP) and left-hand circular polarizations (LHCP). This module enables efficient impedance matching and balanced transmission in QFH antenna configurations.

![QFH antenna balun](/doc/src/img/QFHBAL01.png)

## Key Features

- **Polarization**: RHCP and LHCP
- **Frequency Range**: 4.5 - 3000 MHz
- **Insertion Loss**: 2 dB typical
- **Amplitude Balance**: ±1 dB
- **Phase Balance**: ±20°
- **Power Rating**: 250 mW max RF, 30 mA max DC
- **Operating Temperature**: -55 °C to +85 °C
- **Dimensions**: Diameter 32 mm, Height 20 mm
- **Weight**: 10 g

## Transformer Mounting Options

The **ETC1-1-13** transformer on the QFHBAL01 module can be soldered onto the PCB in two configurations:

1. **Galvanic Isolation**: Isolates the antenna from the RF line, enhancing protection for the receiver input but potentially increasing insertion loss slightly.
2. **Direct Galvanic Connection**: Connects the antenna directly to the RF line without isolation, minimizing insertion loss but offering less protection for the receiver input.

These configurations allow customization based on application requirements for input protection and insertion loss.

### Balun Polarization and Connection

![Balun connection](https://uuki.kapsi.fi/pix/qha/qha-diagram_medium.png)

| Helices     | Feedpoint      | Radiation | Polarization |
|-------------|----------------|-----------|--------------|
| Left-hand   | Standard       | Upward    | RHCP         |
| Right-hand  | Anti-standard  | Upward    | LHCP         |
| Left-hand   | Anti-standard  | Downward  | RHCP         |
| Right-hand  | Standard       | Downward  | LHCP         |

*Source: [QHA Simulation](https://uuki.kapsi.fi/qha_simul.html)*

## Schematic and Mechanical Drawing

- [Schematic (PDF)](/doc/gen/QFHBAL01-schematic.pdf)
- [Mechanical Drawing (PDF)](/doc/src/img/dimensions.png)

### ETC1-1-13 Transformer Specifications

The **ETC1-1-13** transformer offers a 1:1 impedance ratio suitable for balanced RF transmission:

- **Frequency Range**: 4.5 - 3000 MHz
- **Insertion Loss**: 0.32 dB typical, max 3.5 dB at high frequencies
- **Amplitude Balance**: ±1 dB
- **Phase Balance**: ±20°
- **Power Rating**: 250 mW max
- **Operating Temperature**: -55°C to +85°C

