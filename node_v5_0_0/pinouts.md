| RP2040 GPIO | External Connection | Function/Peripheral | Remarks                       |
| ----------- | ------------------- | ------------------- | ----------------------------- |
| 0           |                     | SIM7080G TX0        |                               |
| 1           |                     | SIM7080G RX0        |                               |
| 2           |                     | PCF8523 MFP1        |                               |
| 3           |                     | PCF8523 MFP2        |                               |
| 4           | SDA                 | I2C0 SDA            | RTC & EEPROM on this i2c      |
| 5           | SCL                 | I2C0 SCL            | RTC & EEPROM on this i2c      |
| 6           |                     | SP3485 DE           |                               |
| 7           |                     | SP3485 !RE          |                               |
| 8           | TX1                 | SP3485 DI           | sp3485 on this uart           |
| 9           | RX1                 | SP3485 RO           | sp3485 on this uart           |
| 10          |                     | RFM69 DIO0          |                               |
| 11          |                     | RFM69 DIO1          |                               |
| 12          |                     |                     | not connected.                |
| 13          |                     | 5V REG ENABLE       |                               |
| 14          |                     | SIM7080G PWRKEY     |                               |
| 15          |                     | SIM7080G DTR        |                               |
| 16          | MISO                | SPI0 MISO           |                               |
| 17          |                     | RFM69 CS            |                               |
| 18          | CLK                 | SPI0 CLK            |                               |
| 19          | MOSI                | SPI0 MOSI           |                               |
| 20          |                     | RFM69 RST           |                               |
| 21          | CS                  |                     | can be any GPIO func.         |
| 22          |                     | RFM69 DIO2          |                               |
| 23          |                     | RFM69 DIO3          |                               |
| 24          |                     | RFM69 DIO4          |                               |
| 25          |                     | RFM69 DIO5          |                               |
| 26          |                     | VBAT SAMPLE         | 1/2 voltage divider from VBAT |
| 27          | GP27 (ADC1)         |                     |                               |
| 28          | GP28 (ADC2)         |                     |                               |
| 29          | GP29 (ADC3)         |                     |                               |
