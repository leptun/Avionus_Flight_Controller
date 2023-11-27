# Avionus_Flight_Controller

This repo contains the mainboard for the Avionus project, a semi-autonomous plane/drone. The project is work in progress 🚧.

Features:
- STM32F722ZE MCU with hardware float, 512KB of flash and 256KB of RAM
- 16MB total of external dual-mode QuadSPI (QPI) flash memory with XIP capability
- Full size SD card slot
- GPS (ublox MAX-M10S) with onboard antenna
- 9dof IMU ICM-20948
- LIDAR distance sensors with headers for:
  - LIDAR07-100W
  - VL53L1X
- 16 servo outputs (including at least one UART connection)
- RC remote input:
  - PPM interface
  - iBus interface
- LoRa 868MHz module using Semtech SX1262
- USB 2.0 FS with Type C connector (device only)
- Independent power domanins for the peripherals:
  - Power domains voltage measurement and monitoring
  - Current measurement of critical power domains
  - Very low power shutdown with wake from RTC
  - ESD protection of all IO
- STDC14 debugging header for STLINK-V3:
  - SWD
  - JTAG
  - SWO
  - UART
