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
  2. Additional 2.54mm pitch header with VCC, GND, UART, PPS and I2C
  3. PPS LED
  4. TX/RX LEDs

## Module Design Choices

### v1.0

- PCB
  - 2 layer
  - Test pads on user visible side (satisfies A6)
  - 20x35mm form factor (satisfies A1)
  - Silk screen on user visible side with checkable baud rate options
- Connectors
  - UFL Antenna connector (satisfies A5)
  - 2.54mm pitch header with VCC, GND, UART, PPS and I2C (satisfies C2)
- Battery backup with 6.8mm SDM 3V rechargeable lithium cell (satisfies B2)
- GPS Module : [u-blox MAX-M10](https://www.u-blox.com/en/product/max-m10-series?legacy=Current#Documentation-&-resources) (can satisfy A1, A2, A3 with regulator, A4, B1, B2, B3 and C1)
- LEDs on user visible side (satisfies C3 and C4)
- No antenna short circuit detection (does not satisfy B3 or C1)
- Constant 5V antenna supply (satisfies A4, but not B1)

Specific components

- [u-blox MAX-M10](https://www.u-blox.com/en/product/max-m10-series?legacy=Current#Documentation-&-resources)
- Battery : [SEIKO INSTRUMENTS MS518SE-FL35E](https://www.farnell.com/datasheets/3115182.pdf) ([Farnell](https://be.farnell.com/en-BE/seiko-instruments/ms518se-fl35e/battery-button-lithium-3-4mah/dp/3534575))
- U.FL : [HIROSE(HRS) U.FL-R-SMT-1(10)](https://www.farnell.com/datasheets/2691132.pdf) ([Farnell](https://be.farnell.com/en-BE/hirose-hrs/u-fl-r-smt-1-10/rf-coaxial-u-fl-straight-jack/dp/1688077))
- C1, C2 : [0603B105K250NT](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_FH--Guangdong-Fenghua-Advanced-Tech-0603B105K250NT_C59302.pdf)
- L1 (Antenna supply inductor, 27nH) : [Murata LQG15HS27NJ02D](https://www.mouser.be/datasheet/2/281/1/JELF243B_0010-1699614.pdf)
- C4, C5, C6 (Antenna supply filter, 10nF, 16V, X7R) : [CC0603KRX7R0BB103](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_YAGEO-CC0603KRX7R0BB103_C107059.pdf)
- 3.3V Regulator : [SPX5205M5-L-3-3/TR](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_MaxLinear-SPX5205M5-L-3-3-TR_C6864.pdf)
- D1 : [RB551V-40](https://www.lcsc.com/datasheet/lcsc_datasheet_2308281443_hongjiacheng-RB551V-40_C7502699.pdf)
- D2 : [KINGBRIGHT KPTR-3216SURCK](https://www.farnell.com/datasheets/2045968.pdf)
- D3 : [XL-3216SURC](https://www.lcsc.com/datasheet/lcsc_datasheet_2402181505_XINGLIGHT-XL-3216SURC_C965822.pdf)
- D4, D5 : [XL-3216UOC](https://www.lcsc.com/datasheet/lcsc_datasheet_2402181505_XINGLIGHT-XL-3216UOC_C965823.pdf)
- R1 : [ERJPA3J100V](https://www.lcsc.com/product-detail/Chip-Resistor-Surface-Mount_PANASONIC-ERJPA3J100V_C441879.html)
- R2, R3, R4 : [CR0603-FX-3301ELF](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_BOURNS-CR0603-FX-3301ELF_C203527.pdf)
- R5, R6, R7, R8 : [RC0603JR-07220RL](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_YAGEO-RC0603JR-07220RL_C114683.pdf)
