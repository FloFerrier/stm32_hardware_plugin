# stm32_hardware_plugin
## Description
- Version : OPENPILL v1.0
- Based on NucleoF446RE board
## Functionalities
- 2 User leds
- 6 connectors to I2C1
- 2 connectors to UART2
- Connector for SWD
- Connector for connecting external power (refer to Nucleo datasheet)
- Enable external power E5V on Nucleo board (jumper on JP5)
- Jumper for external power or routing a INA219 sensor for power measurement
- Module BLE : RN4871
## Bugs
- External power not correct (change 5v by E5V or VIN on input Nucleo board)
