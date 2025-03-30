
## Team Bytes
| Byte | Function |
|----|-------|
| AZ | Start |
| YB | Stop  |

| Unique ID | Byte |
|-----|-----|
|Shon Ha| H |
|Maximus Mathews|M|
|Rohan Fernandez|F|
|Shelton Larance|L|

---------------------
## Sent Messages:

**Message Type 1: Toggle Manual/automatic modes**
* Incoming toggle data that will decide if the sensor data or button data drives the motors, data will be sent to sensor system

|               | Byte 1      | Byte 2 |
|---------------|-------------|--------|
| Variable Name | mode | mode_toggle |  
| Variable Type | char    |  uint8_t| 
| Min Value     | M           |   0|
| Max Value     | M           |   1|
| Example       | M           |   1|


**Message Type 5: Directional button data transmission**
* allows for left/right manual motor control if manual mode is on, originates in HMI

|               | Byte 1      | Byte 2       | Byte 3    |  Byte 4 |
|---------------|-------------|--------------|-----------|----------
| Variable Name | L        | button_left |   R     | button_right|
| Variable Type |  char    | uint8_t      | char        |  uint8_t |
| Min Value     | L          | 0            | R         |  0       |
| Max Value     | L          | 1            | R         |  1       |
| Example       | L          | 1            | R         |  1       |

----------------
## Kept Messages: 
**Message Type 3: Voltage Readings for display** 
* Should match the output from the MQTT but appears on the physical LCD (incoming data)
* Data will be acquired from all 4 different sensors for a total of 16 bytes from all 4 combined

|               | Byte 1         | Byte 2-3        |  
|---------------|----------------|-----------------|  
| Variable Name | voltage_sensor | voltage_reading |  
| Variable Type | char           | uint16_t        |  
| Min Value     | S1, S2, S3, S4 | 0000            |  
| Max Value    | S1, S2, S3, S4 | 5400            |  
| Example S1) | S1             | 3300            |  
| Example (S2)  | S2            | 4200            |  
| Example (S3) | S3             | 2750            |  
| Example (S4)  | S4             | 5000            |  
