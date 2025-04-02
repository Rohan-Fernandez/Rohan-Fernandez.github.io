
## Team Bytes
| Byte | Function |
|----|-------|
| AZ | Start |
| YB | Stop  |

| Unique ID | Byte |
|-----|-----|
|Shon Ha| h |
|Maximus Mathews|m|
|Rohan Fernandez|f|
|Shelton Larance|l|

**For my messages: incoming = lf, outgoing = fm
---------------------
## Incoming Messages:

* **Part 1 - Bytes 1 and 2: Toggle Manual/automatic modes**
* Incoming toggle data that will decide if the sensor data or button data drives the motors, data will be sent to sensor system
*sent out to next team member after being recieved
* **Part 2 - Bytes 3-7: Voltage Readings for display** 
* Should match the output from the MQTT but appears on the physical LCD (incoming data)
* Data will be acquired from all 4 different sensors for a total of 16 bytes from all 4 combined
* Does not get sent out again

|                |  Byte 1        | Byte 2          | Byte 3         | Byte 4-7        |
|--------------- |--------------- |--------------- |----------------|-----------------|
| Variable Name  | mode           | mode_toggle    | voltage_sensor | voltage_reading |
| Variable Type  | char           | char           | char           |  char           |
| Min Value      | M              | 0              | V              | 0000            |
| Max Value      | M              | 1              | V              | 5400            |
| Example        | M              | 1              | V              | 2572            |

----------------------
## Outgoing Messages:

**Part 1 - Bytes 1-2: Mode Toggle**
* Incoming toggle data that will decide if the sensor data or button data drives the motors, data will be sent to sensor system
  
**Part 2 Bytes 3-6: Directional button data transmission, coming from HMI (my system)**
* allows for left/right manual motor control if manual mode is on, originates in HMI
  


|               | Byte 1    | Byte 2      | Byte 3      | Byte 4       | Byte 5    |  Byte 6 |
|---------------|---------- |---------- |-------------|--------------|-----------|---------|
| Variable Name | mode      |  mode_toggle         | L        | button_left |   R     | button_right|
| Variable Type | char      |   char             |  char    | char     | char        | char |
| Min Value     | M         |   0          | L          | 0            | R         |  0       |
| Max Value     | M         |   1         | L          | 1            | R         |  1       |
| Example       | M         |   1           | L          | 1            | R         |  1       |

----------------
