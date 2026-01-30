# Smart-Ring


## Overview
This project focuses on developing a smart ring that integrates multiple sensors to monitor physiological and environmental parameters in real time. The device is designed to be non-intrusive and energy efficient, making it suitable for long-term wearable use.

The smart ring collects sensor data locally and is designed to transmit it via Bluetooth Low Energy (BLE) to external devices such as smartphones for further analysis.

## Key Features
- Multi-sensor health monitoring
- Low-power embedded system design
- Compact wearable form factor
- Sensor fusion for improved signal reliability

## Hardware Components
- Microcontroller:nRF52832 (BLE-enabled, low power)
- PPG Sensor: MAX30101 (heart rate & SpO₂)
- IMU: ICM-20948 (9-axis motion tracking)
- Temperature Sensor: DS18B20
- Air Quality Sensor: CCS811 

## Firmware Development
- Initial development attempted using **Segger Embedded Studio** and **nRF Connect**
- Due to detection issues, firmware was successfully implemented using **Arduino IDE**


## Technical Challenges
- Lack of native Arduino library support for MAX30101
- Modified MAX30105 library to support MAX30101 detection
- Motion artifacts affecting PPG signal quality
- Power optimization for wearable constraints

## Results
- Successful real-time data acquisition from all sensors
- Stable temperature and air quality readings
- IMU data used to identify motion-related noise in PPG signals
- Multi-sensor approach validated for wearable health monitoring

## Future Work
- Full BLE implementation and mobile app integration
- Flexible PCB (FPCB) design
- Battery optimization and enclosure miniaturization
- Advanced signal processing and anomaly detection

## Applications
- Continuous health monitoring
- Early detection of physiological irregularities
- Fitness and wellness tracking
- Remote healthcare support

