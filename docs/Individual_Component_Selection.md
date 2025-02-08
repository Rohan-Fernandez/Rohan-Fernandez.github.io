---
title: Individual Component Selection
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

 <img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/MFG_NHD-C0220BiZ-FS(RGB)-FBW-3VM.jpg?raw=true">

* $14.46/each
* [link](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-C0220BIZ-FS-RGB-FBW-3VM/3507740)
    
| Pros                                      | Cons                                                              |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Specifically designed for I2C             | Fairly expensive, especially if multiple needed              |
| Good Datasheet with accessible key commands  | Shipping could be a problem, espeically with added tariff |
| RGB backgrounds to make text appear more clearly | 

2. AMC0802BR-B-Y6WFDY-I2C

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/AMC0802BR-B-Y6WFDY-I2C.jpg?raw=true">

 * $8.49/each
 * [link](https://www.digikey.com/en/products/detail/orient-display/AMC0802BR-B-Y6WFDY-I2C/22531880)
    
| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Specifically designed for I2C             | Much less display space compared to other options            |
| Cost effective                            | Might require separate voltage regulation from other parts (higher voltage) |
| Physically smaller (less space on board) | 

3. NHD-0216AW-IB3

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/NHD-0216AW-IB3.jpg?raw=true">

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

1. 3491 (Adafruit Pushbutton)

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/MFG_3491.jpg?raw=true">


 * $2.50/each
 * [link](https://www.digikey.com/en/products/detail/sparkfun-electronics/PRT-14460/7915747)
    
| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Includes a built-in LED, making it easier to identify the button's state | Rather expensive cost per button           |
| Larger button for easier pressing          | The LED light is dimmer when run at 3.3 V |
| Works with a decent range of voltages, so no specific regulation is required |

2. PRT-14460 (Spark-fun Electronics)

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/PRT-14460.jpg?raw=true">

 * $1.75 per pack: $0.44 per button
 * [link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3491/7349497)
    
| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Very inexpensive | Datasheet with very minimal information          |
| Each button is a different color to distingush between functions | Buttons might be a bit small and difficult for accurate pressing|
| 4 are in each pack, so there's potentially one spare |

3. 1010 (Adafruit square button pack)

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/1010.jpg?raw=true">

 * $5.95 per pack: $0.40 per button
 * [link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/1010/7244937)
    
| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Square buttons that are easy to press, so a young student can easily press/use them | Datasheet with very little useful information   |
| Multiple colors and many spares | Only comes in a large pack, so more buttons than needed and higher cost, despite low cost per button|

**Choice:** Option 2: PRT-14460 (Spark-fun Electronics)

**Rationale:** These buttons are the best choice for the purposes of this project due to their low cost, as this component is not particularly important to the workings of the project, with others needing to take higher priority, though colored buttons would help its overall cohesion and presentation.


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
| Absolute Maximum current <br> (for entire IC) | Vss = 350 mA, Vdd = 250 mA    | as found in datasheet                                                                                     |
| Maximum GPIO current <br> (per pin)           | ±50 mA      | as found in datasheet                                                                                     |
| Supports External Interrupts?                 | Yes      | as found in datasheet                                                                                     |
| Required Programming Hardware, Cost, URL      | Various info regarding the hardware: [link](https://www.microchip.com/en-us/product/PIC18F27Q10)     | found on the microcontroller's product page                                                               |
| Works with MPLabX?                            | Yes     | Required.  See [Microchip Development Tools](https://www.microchip.com/development-tools)                 |
| Works with Microchip Code Configurator?       | Refer to Screenshot Below      | Can be validated in MPLabX.  Screenshot required.                                                         |

<img src="https://github.com/Rohan-Fernandez/Rohan-Fernandez.github.io/blob/main/Images/V2PIC_Pinout.png?raw=true">

As shown in the above screenshot, in mplabx I was able to set up the currently necessary pins for my section of the project and then successfully build it. The main pins are RC3 and RC4 for the I2C SCL and SDA pins respectively along with 3 GPIOs (RA1, RA2, RA3)vconfigured to input, which represent the 3 buttons that will be involved with user controlled motor movement. A 4th might be added depending on available resources in other parts of the project, for more dynamic side to side motion, which is doable by just adding one extra GPIO button pin. Additonally UART pins ar present to account for communication between devices in the project.

| Module | # Available | Needed | Associated Pins (or * for any) |
| ---------- | ----------- | ------ | ------------------------------ |
| GPIO       | 24           | 3      | RA1, RA2, RA3                              |
| ADC        | 24          | 0      | NA                             |
| UART       | 2           | 1      | RC6, RC7                              |
| SPI        | 2           | 0      | NA                             |
| I2C        | 2           | 1      | RC3, RC4                             |
| PWM        | 2           | 0      | NA                             |
| ICSP       | 2           | 1      | MCLR = RE3 (and RB6, RB7)                             |
| ...        | ...         | ...    | ...                            |


