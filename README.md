# RISC-V core industrial-grade interconnected microcontroller CH32V407_V467
EN | [中文](README_zh.md)



### Overview
CH32V407 is an industrial-grade interconnected microcontroller designed based on the Qingke RISC-V core. It supports zero-wait operation at a main frequency of 200MHz and supports the V vector instruction set for applications such as accelerated computing or parallel processing. CH32V407 is equipped with two sets of USB 2.0 high-speed PHY transceivers (480Mbps), an Ethernet MAC controller, and a 10/100M physical layer transceiver; it also includes built-in dual ADC units, dual DAC units, OPA operational amplifiers, and other analog resources. It provides a rich set of peripheral resources, including two sets of 24-channel DMA controllers, SDIO, DVP digital image interface, RNG, ARGB, LTDC, FSMC, multiple sets of timers, 10 sets of USART serial ports, I2C interface, I3C interface, three sets of SPI, two sets of I2S, and CAN interface. Based on CH32V407, CH32V467 adds 4M or 8M bytes of on-chip extended PSRAM memory, which supports DMA.


### System Block Diagram
![Alt](image/frame.png)
### Features

- Qingke 32-bit RISC-V3V core, featuring a combination of multiple instruction sets
- Supports V vector instruction set and parallel computing
- Fast programmable interrupt controller + hardware interrupt stack
- Level 2 interrupt nesting
- The system's main frequency is up to 200MHz

- 200KB zero-wait volatile data storage area SRAM
- 992KB program storage area CodeFlash
  (Zero-wait application area + non-zero-wait data area)
- 28KB system bootloader storage area BootLoader
- 128B user-defined information storage area

- 8MB extended PSRAM memory (only for CH32V467)
- DMA block read/block write speed can reach up to 800Mbytes/s

- System power supply VDD voltage range: 2.9~3.6V
- Low power consumption modes: sleep, halt, standby
- VBAT power supply independently powers the RTC and backup registers

- Built-in factory-calibrated 20MHz RC oscillator
- Built-in RC oscillator with a frequency of approximately 40kHz
- The high-speed oscillator supports an external crystal ranging from 5 to 32 MHz
- The low-speed oscillator supports an external 32.768kHz crystal
- Power-on/power-off reset, programmable voltage monitor
- Real-time clock (RTC): 32-bit independent timer

- 2 sets of 12-bit digital-to-analog converters (DACs)

- 2 sets of 12-bit analog-to-digital converters (ADCs):
- Analog input range: VSSA to VDDA
- 16 channels of external signals + 2 channels of internal signals
- Dual ADC conversion mode

- Operational amplifier (OPA)/Programmable Gain Amplifier (PGA)/Voltage comparator:
- Each with 2 input channels and output channels

- 2 sets of 24-channel universal DMA controllers

- 10 sets of USART serial ports: support LIN

- I2C interface (supporting SMBus/PMBus)

- I3C interface

- 3 sets of SPI interfaces (SPI2 and SPI3 are used for I2S2 and I2S3)

- 2 sets of 480Mbps high-speed USB 2.0 controllers and PHYs:
- Supports high-speed/full-speed Host and Device modes
- Supports 1024-byte data packets

- CAN interface (2.0B active)

- SDIO interface (MMC, SD/SDIO cards, and CE-ATA)

- FSMC memory interface

- 150MHz digital video interface DVP

- LCD-TFT display controller LTDC

- Random Number Generator (RNG)

- Addressable RGB (ARGB)

- 100M Ethernet controller MAC and 10M/100M PHY
- MAC and PHY are fully integrated, with only capacitors required as peripherals
- Supports Auto-MDIX automatic line conversion and polarity self-adaptation
- 10M/100Mbps auto-negotiation, supporting both full-duplex and half-duplex

- Multiple sets of timers:
- 2x16-bit advanced timers, supporting dead zone control and emergency
  Brake, providing complementary PWM output for motor control
- 4 16-bit general-purpose timers, providing input capture/output comparison
  Comparison/PWM/pulse counting and incremental encoder input
- 2 basic timers
- 2 watchdog timers (independent and window type)
- System time base timer: 32-bit counter

- Fast GPIO port:
- 77 I/O ports, mapped to 16 external interrupts

- Security features: CRC calculation unit, 96-bit unique chip ID

- Single-line or dual-line debugging mode

- Packaging type: LQFP, QFN
