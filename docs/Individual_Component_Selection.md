---
title: Individual_Component_Selection.
---
---
Part 1: Component Selection
---
**PIC Microcontrollers**

1. PIC16F15213T

    <img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/PIC16F15213T.jpg?raw=true">

    * $0.50/each
    * [link](https://www.digikey.com/en/products/detail/microchip-technology/PIC16F15213T-I-MF/12807572)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Supports UART and I2C                     | Will be difficult to solder due to size and type            |
    | Very small and cost effective             | Not flexible for project changes or errors                  |
    | Meets surface mount requirements |

2. PIC18F27Q10-I/SO

    <img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/PIC18F27Q10.jpg?raw=true">

    * $1.45/each
    * [link](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F27Q10-I-SO/10064343)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Supports UART and I2C                     | Will need its specs to be closely monitored in the datasheet (specific voltages, etc.) |
    | Good memory and general specs             | Chip's length might create spacing concerns                                         |
    | Surface mount version to meet project requriements, more space-economical than 40 pin version |

3. PIC18F14Q20-I/SS

    <img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/PIC18F14Q20.jpg?raw=true">
   
    * $0.92/each
    * [link](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F14Q20-I-SS/24617052)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Supports UART and I2C, also similar to what was used in class| Small amount of memory, can pose serious issues, especially with the already fairly slow I2C |
    | Very cost-effective                       | Comparitively lower capabilities                     |
    | Meets surface mount constraint of project | Described as a new component, may be buggier than more tested/older ones


**Choice:** Option 2: PIC18F27Q10-I/SO

**Rationale:** The PIC18F27Q10 was selected due to it being cost-effective while also providing solid capabilities compared to the other options. The 28 pins will allow for potetntial additions as the project's inclusions are adjusted and it meets my sub-system's specific need for I2C (for a screen interface).

**Display Screens**

1. NHD-C0220BIZ-FS(RGB)-FBW-3VM

 Image

    * $14.46/each
    * [link](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-C0220BIZ-FS-RGB-FBW-3VM/3507740)
    
    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Specifically designed for I2C             | Fairly expensive, especially if multiple needed              |
    | Good Datasheet with accessible key commands  | Shipping could be a problem, espeically with added tariff |
    | RGB backgrounds to make text appear more clearly | 

2. AMC0802BR-B-Y6WFDY-I2C

Image

    * $8.49/each
    * [link](https://www.digikey.com/en/products/detail/orient-display/AMC0802BR-B-Y6WFDY-I2C/22531880)
    
    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Specifically designed for I2C             | Much less display space compared to other options            |
    | Cost effective                            | Might require separate voltage regulation from other parts (higher voltage) |
    | Physically smaller (less space on board) | 

3. NHD-0216AW-IB3

Image

    * $28.49/each
    * [link](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-0216AW-IB3/6198749)
    
    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Specifically designed for I2C             | Very expensive, can likely one order one            |
    | Wide voltage range                        | No Backlight is included |
    | More visually pleasing OLED Screen, rather than a more simplistic LCD |

**Choice:** Option 1: NHD-C0220BIZ-FS(RGB)-FBW-3VM

**Rationale:** The NHD-C0220BIZ-FS(RGB)-FBW-3VM was selected due to it being a good balance of cost and effectiveness, as it has fairly solid display capapbilities and should be able to show important data while also being able to be smoothly integrated with the rest of the system (voltage, spacing, I2C, etc.).

**Push-Buttons**

1. 


---
Part 2 Microcontroller (PIC) Selection:
---
| PIC Info                                      | Answer | Help                                                                                                      |
| --------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- |
| Model                                         | PIC18F27Q10 | Include the entire part number (leave off any letters at the end that specify the package type)           |
| Product Page URL                              | [link](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F27Q10-I-SO/10064343)     | Do not paste links directly into the table.  Use a [link](#)                                              |
| Datasheet URL(s)                              | [link](https://ww1.microchip.com/downloads/en/DeviceDoc/PIC18F27-47Q10-Data-Sheet-40002043E.pdf)      | Do not paste links directly into the table.  Use a [link](#)                                              |
| Application Notes URL(s)                      | [link](https://www.microchip.com/en-us/search?searchQuery=PIC18F27Q10&category=Application%20Notes&fq=start%3D0%26rows%3D21)      | Do not paste links directly into the table.  Use a [link](#)                                              |
| Vendor link                                   |[link](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F27Q10-I-SO/10064343)     | Digikey, Jameco, etc.  Do not paste links directly into the table.  Use a [link](#)                       |
| Code Examples                                 | [link](https://github.com/microchip-pic-avr-examples/pic18f47q10-cnano-i2c-read-write-int-bare)     | url(s) for libraries on github or other sites related to the microcontroller and your planned peripherals |
| External Resources URL(s)                     | Specifically for LCD interface: [link](https://www.youtube.com/watch?v=1LqUljBXLqw&pp=ygUMI3BpYzE4ZjQ1NDUw)      | Search on Google and YouTube for other resources for each specific microcontroller.                       |
| Unit cost                                     | $1.45     | Find in the Microchip online store, or Digikey                                                            |
| Absolute Maximum Current for entire IC        | 350 mA for Vss    | Find in the microcontroller datasheet                                                                     |
| Supply Voltage Range                          | 1.8 V - 5.5V       | Min / Nominal / Max / Absolute Max, as found in datasheet                                                 |
| Absolute Maximum current <br> (for entire IC) | ?      | as found in datasheet                                                                                     |
| Maximum GPIO current <br> (per pin)           | ±50 mA      | as found in datasheet                                                                                     |
| Supports External Interrupts?                 | Yes      | as found in datasheet                                                                                     |
| Required Programming Hardware, Cost, URL      | ?      | found on the microcontroller's product page                                                               |
| Works with MPLabX?                            | Yes     | Required.  See [Microchip Development Tools](https://www.microchip.com/development-tools)                 |
| Works with Microchip Code Configurator?       | ?      | Can be validated in MPLabX.  Screenshot required.                                                         |


| Module | # Available | Needed | Associated Pins (or * for any) |
| ---------- | ----------- | ------ | ------------------------------ |
| GPIO       | 25           | 3      | ?                              |
| ADC        | ?           | ?      | ?                              |
| UART       | ?           | ?      | ?                              |
| SPI        | ?           | ?      | ?                              |
| I2C        | ?           | ?      | ?                              |
| PWM        | ?           | ?      | ?                              |
| ICSP       | 2           | 1      | ?                              |
| ...        | ...         | ...    | ...                            |


