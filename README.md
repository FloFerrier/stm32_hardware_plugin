# stm32_hardware_plugin
## Description
- Version : OPENPILL v1.0
- Supported hardware : Nucleo-F446RE board
- EasyEDA files : PCB.json and Schematic.json
## Functionalities
- 2 User leds
- 6 connectors to I2C1
- 2 connectors to UART2
- Connector for SWD
- Connector for connecting external power (refer to Nucleo datasheet)
- Enable external power E5V on Nucleo board (jumper on JP5)
- Jumper for external power or routing a INA219 sensor for power measurement
- Module Bluetooth Low Energy : RN4871
## Mapping
| Board Pin Name | STM32 Pin Name |              |
|----------------|----------------|--------------|
| RN4871_RX      | PC10           | UART3_TX     |
| RN4871_TX      | PC11           | UART3_TX     |
| RN4871_MODE    | PC9            |              |
| SWDIO          | PA13           |              |
| SWCLK          | PA14           |              |
| NRST           | RESET          |              |
| SWO            | PB3            |              |
| LED2           | PC1            |              |
| LED1           | PC0            |              |
| SCL1           | PB8            | I2C1_SCL     |
| SDA1           | PB9            | I2C1_SDA     |
| TX2            | PA2            | UART2_TX     |
| RX2            | PA3            | UART2_RX     |
## Bugs
- External power not correct (change 5v by E5V or VIN on input Nucleo board)
