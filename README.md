# Smart Real-Time Weather Monitoring System Using IoT

## Overview

The **Smart Real-Time Weather Monitoring System** is an IoT-based project that monitors and displays environmental parameters like temperature, humidity, light intensity, and rainfall in real time. The system uses various sensors and displays the collected data on an LCD. It also transmits the data wirelessly for remote monitoring.

## Features

- **Real-Time Data Monitoring**: Measures temperature, humidity, light intensity, and rainfall.
- **LCD Display**: Local display of sensor data.
- **IoT Connectivity**: Sends data to a cloud server for remote access.
- **Efficient Power Usage**: Uses a 5V external power supply.

---

## Components

1. **NodeMCU ESP8266**: Microcontroller with built-in WiFi for IoT connectivity.
2. **DHT11 Sensor**: Measures temperature and humidity.
3. **LDR Sensor**: Detects light intensity.
4. **Rain Sensor**: Detects rainfall presence.
5. **I2C Module**: Enables easy communication between NodeMCU and LCD.
6. **16x2 LCD Display**: Displays sensor data.
7. **5V DC External Power Supply**: Powers the entire system.

## Connections

### Sensors:
- **DHT11 Sensor**:
  - VCC → 3V3 on NodeMCU
  - GND → GND on NodeMCU
  - OUT → D5 on NodeMCU

- **LDR Sensor**:
  - VCC → 3V3 on NodeMCU
  - GND → GND on NodeMCU
  - OUT → D6 on NodeMCU

- **Rain Sensor**:
  - VCC → 3V3 on NodeMCU
  - GND → GND on NodeMCU
  - OUT → D7 on NodeMCU

### Display:
- **I2C Module**:
  - VCC → 3V3 on NodeMCU
  - GND → GND on NodeMCU
  - SDA → D2 on NodeMCU
  - SCL → D1 on NodeMCU

---

## How to Use

1. **Hardware Setup**:
   - Connect the components as per the circuit diagram.

2. **Software Setup**:
   - Install the Arduino IDE.
   - Add the ESP8266 board to the IDE.
   - Install required libraries (`DHT`, `Wire`, `LiquidCrystal_I2C`).
   - Upload the code to the NodeMCU.

3. **IoT Setup**:
   - Configure WiFi credentials in the code.
   - Use the blynk app

4. **Power the System**:
   - Provide 5V DC power to the system.

---

## Applications

- Weather monitoring stations
- Smart agriculture
- Environmental monitoring
- Home automation

---

## Troubleshooting

1. **No Data on LCD**:
   - Check I2C connections.
   - Ensure the correct I2C address in the code.

2. **WiFi Not Connecting**:
   - Verify WiFi credentials.
   - Check NodeMCU firmware.

3. **Incorrect Sensor Readings**:
   - Ensure proper connections.
   - Test individual sensors.

---

## Future Enhancements

- Add more sensors (e.g., air quality, wind speed).
- Integrate with mobile apps for better usability.
- Use solar panels for power supply.

---

## License

This project is open-source and can be freely modified or distributed.
