# ICOM Internal modules

A collection of custom internal modules for ICOM IC-F5060/6060 radios.

## Pinouts

The IC-F5060/6060 and IC-F3162T radios have two 20-pin accessory connectors (J1 and J2). They mate with a [Panasonic P5 Series P5K AXK640347YG](https://na.industrial.panasonic.com/products/connectors/board-board-connectors/lineup/narrow-fine-pitch-connectors/series/82696/model/83045) connector.  
You can find a KiCAD Library for J1 and J2 [here](./CAD-Libs/ICOM-J1-J2). The pinouts are as follows (from the service manual) :

### J1

```ascii
           ┌─────╮
      NC   │40  1│   NC
     GND   │39  2│   GND
     +5V   │38  3│   PTTI
     VCC   │37  4│   PTTO
      NC   │36  5│   MCOT
   MMUTI   │35  6│   NC
    AFON   │34  7│   MCIN
    BEPO   │33  8│   NC
    RMUT   │32  9│   NC
    DISC   │31 10│   NC
   AFOUT   │30 11│   NC
      NC   │29 12│   BUSY
     REM   │28 13│   SIGO
     CCS   │27 14│   OPT1/RxD
    CIRQ   │26 15│   OPT2/TxD
      NC   │25 16│   OPT3
     CSO   │24 17│   GND
     CSI   │23 18│   OPV3
     CCK   │22 19│   OPV2
      NC   │21 20│   OPV1
           └─────╯
```

### J2

```ascii
           ┌─────╮
     DIF   │40  1│   DIF
     GND   │39  2│   GND
     +5V   │38  3│   NC
      8V   │37  4│   NC
      NC   │36  5│   NC
      NC   │35  6│   DMO
      NC   │34  7│   NC
      NC   │33  8│   DMI
      NC   │32  9│   NC
    DISC   │31 10│   VREF
      NC   │30 11│   NC
    DAFO   │29 12│   NC
      NC   │28 13│   NC
     CCS   │27 14│   OPT1 (DPDN)
    CIRQ   │26 15│   OPT2 (DRES)
      NC   │25 16│   OPT3 (DRES)
     CSO   │24 17│   GND
     CSI   │23 18│   NC
     CCK   │22 19│   GND
     GND   │21 20│   GND
           └─────╯
```

## Acknowledgements

Made with ❤️, lots of ☕️, and lack of 🛌  
Published under CreativeCommons BY-SA 4.0

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)  
This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
