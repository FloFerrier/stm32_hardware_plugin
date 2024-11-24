# stm32_hardware_plugin
## Description
- Version : OPENPILL v2.0
- Supported hardware : Nucleo-F446RE board
- EasyEDA files : PCB.json and Schematic.json
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
## Mapping
| Board Pin Name | STM32 Pin Name |              |
|----------------|----------------|--------------|
| RN4871_RX      | PC10           | UART3_TX     |
| RN4871_TX      | PC11           | UART3_TX     |
| LED3           | PB0            |              |
| LED2           | PC1            |              |
| LED1           | PC0            |              |
| I2C1_SCL       | PB8            |              |
| I2C1_SDA       | PB9            |              |
| SPI2_MISO      | PC2            |              |
| SPI2_MOSI      | PC3            |              |
| SPI2_SSEL      | PB12           | SPI2_CS      |
| SPI2_CLK       | PB10           |              |
| ENABLE_PIN     | PA7            |              |
| BUSY_PIN       | PB6            |              |
| RESET_PIN      | PC7            |              |
| ECS_SRAM_PIN   | PA9            |              |
| CMD_PIN        | PA8            |              |
| TX2            | PA2            | UART2_TX     |
| RX2            | PA3            | UART2_RX     |