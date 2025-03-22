## API
----------

## Message Type 1: Toggle Manual/automatic modes
* Button controlled toggle that will decide if the sensor data or button data drives the motors

|               | Byte 1      |  
|---------------|-------------|
| Variable Name | auto_toggle |   
| Variable Type | uint8_t     |   
| Min Value     | 0           |   
| Max Value     | 1           |   
| Example       | 1           |   



## Message Type 3: Voltage Readings for display 
* Should match the output from the MQTT but appears on the physical LCD (incoming data)

|               | Byte 1         | Bytes 2-5        |
|---------------|----------------|-----------------|
| Variable Name | voltage_unit | voltage_value |
| Variable Type | char           | float           |
| Min Value     | V              | 0.000           |
| Max Value     | V              | 5.500           |
| Example       | "V"              | "3.300"           |


## Message Type 5: Directional button data transmission
* allows for left/right manual motor control if manual mode is on

|               | Byte 1      | Byte 2       |
|---------------|-------------|--------------|
| Variable Name | button_left | button_right |
| Variable Type | uint8_t     | uint8_t      |
| Min Value     | 0           | 0            |
| Max Value     | 1           | 1            |
| Example       | 0           | 1            |

