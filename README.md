# stm32_hardware_plugin
## Description
- Version : OPENPILL v2.0
- Based on NucleoF446RE board
## Functionalities
- 3 User leds
- 3 connectors to I2C1
- connector to UART2
- Connector to UART3
- Connector for connecting external power (refer to Nucleo datasheet)
- Enable external power E5V on Nucleo board (jumper on JP5)
- Jumper for external power or routing a INA219 sensor for power measurement
- Module BLE : RN4871
## Changing from v1.0
- Remove SWD connector
- Remove 1 UART2 connector
- Remove 3 I2C1 connectors
- Add 1 UART3 connector
- Add 1 User leds
- Add led for RN4871 module
- Add GND plane on Bottom side
- Fix E5V routage (in place to 5v)
- Change routage (top side only for Nucleo connector)