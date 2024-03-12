# GPS Module

All the files and R&D data for a custom GPS module.

## Module Design Specifications

A.  Must have  

  1. UT-126H form factor (20x35mm)
  2. UART NMEA GPS module with 4800/9600 baud rate
  3. 5V Supply compatible
  4. 5V Antenna supply
  5. UFL Antenna connector
  6. Test pads for VCC, GND, TX, RX and PPS

B.  Nice to have

  1. Switchable antenna supply
  2. Backup battery circuitry
  3. Antenna short circuit detection & protection

C.  Optional

  1. Antenna connection detection
  2. 2.54mm pitch header with VCC, GND, UART, PPS and I2C
  3. PPS LED
  4. TX/RX LEDs

## Module Design Choices

- v1.0
  - PCB
    - 2 layer
    - Test pads on user visible side (satisfies A6)
  - Connectors
    - UFL Antenna connector (satisfies A5)
    - 2.54mm pitch header with VCC, GND, UART, PPS and I2C (satisfies C2)
  - Battery backup with 6.8mm SDM 3V rechargeable lithium cell (satisfies B2)
  - GPS Module : [u-blox MAX-M10](https://www.u-blox.com/en/product/max-m10-series?legacy=Current#Documentation-&-resources) (satisfies A1, A2, A3 with regulator, A4, B1, B2, B3 and C1)
  - LEDs on user visible side (satisfies C3 and C4)
