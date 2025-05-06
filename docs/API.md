
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

**For my messages: incoming = lf, outgoing = fm**

---------------------
## Incoming Messages:

* **Part 1 - Bytes 1 and 2: Toggle Manual/automatic modes**
* Incoming toggle data that will decide if the sensor data or button data drives the motors, data will be sent to sensor system
*   Sent out to next team member after being recieved

 **Part 2 - Bytes 3-8: Sensor 1 for display** 
* Should match the output from the MQTT but appears on the physical LCD (incoming data)
* Data will be acquired from the first of two different sensors, determined by the 2 byte identifier of S1
* Does not get sent out again

 **Part 3 - Bytes 9-14: Sensor 2 for display** 
* Data will be acquired from the second of two different sensors, determined by the 2 byte identifier of S2
* Does not get sent out again

|                |  Byte 1        | Byte 2          | Byte 3-4         | Byte 5-8     | Byte 9-10 | Byte 11-14 |
|--------------- |--------------- |--------------- |----------------|-----------------|-----------|--------|
| Variable Name  | mode           | mode_toggle    | Sensor_1       | sensor_1_value  | Sensor_2 | sensor_2_value|
| Variable Type  | char           | char           | char           |  char           | char     | char         |
| Min Value      | M              | 0              | S1             | 0000            | S2       | 0000          |
| Max Value      | M              | 1              | S1             | 9999            |S2        | 9999          |
| Example        | M              | 1              | S1             | 2572            |S2        | 4572          |

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
