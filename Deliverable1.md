# ICS 4111 – Embedded Systems & IoT
# Semester Project – Deliverable 1

## Student Details

**Name:** William Githinji  
**Admission Number:** 110592  
**Class:** ICS 4B  

**Project Title:** Sunflower Environmental Monitoring System

---

# 1. Environmental Requirements for Sunflower Growth

The table below summarizes the environmental conditions required for proper sunflower growth. These values will be used as reference measurements in the later stages of the project.

| Parameter | Recommended Value |
|---|---|
| Optimal Temperature | 20–30°C |
| Optimal Relative Humidity | 40–70% |
| Recommended Soil Type | Well-drained loamy soil |
| Optimal Soil Moisture Content | 40–60% |
| Optimal Soil pH Range | 6.0–7.5 |
| Suitable Sunlight Exposure | 6–8 hours per day |

---

# 2. Hardware Components

The following hardware components are suitable for developing the sunflower environmental monitoring device.

| Component | Purpose |
|---|---|
| ESP32S DevKit Wi-Fi + BLE Module (30 Pin) | Main microcontroller for reading sensors, processing data and wireless communication |
| DHT22 AM2302 Sensor | Measures environmental temperature and relative humidity |
| MQ-5 Gas Sensor | Detects LPG, methane, butane, propane, natural gas and coal gas |
| 1.3-inch White IIC 128×64 OLED LCD | Displays sensor readings locally |
| 5V 1-Channel Low-Level Trigger Relay Module | Controls an external electrical device |
| Soil Moisture Sensor | Measures soil moisture content |
| Soil pH Sensor | Measures soil acidity or alkalinity |
| Light Sensor/LDR | Estimates sunlight exposure |
| Breadboard | Supports circuit prototyping |
| Jumper Wires | Connects components |
| USB Cable | Powers and programs the ESP32 |
| Resistors | Used for pull-up, current limiting and voltage-divider circuits |
| Capacitors | Stabilize the power supply and reduce electrical noise |
| External Power Supply | Powers components that require a separate supply |

---

# 3. Datasheet and Product Links

| Component | Datasheet / Product Page |
|---|---|
| 1.3-inch White IIC 128×64 OLED LCD | https://www.waveshare.com/wiki/1.3inch_OLED_(A) |
| ESP32S DevKit Wi-Fi + BLE Module | https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32/esp32-devkitc/index.html |
| DHT22 AM2302 Sensor | https://cdn.sparkfun.com/assets/f/7/d/9/c/DHT22.pdf |
| MQ-5 Gas Sensor | https://www.sparkfun.com/datasheets/Sensors/Biometric/MQ-5.pdf |
| 5V 1-Channel Relay Module | https://components101.com/switches/5v-single-channel-relay-module-pinout-features-applications-working-datasheet |

---

# 4. Schematic Designs

## 4.1 Architecture A

Architecture A consists of one ESP32S connected to one MQ-5 gas sensor, one DHT22 temperature and humidity sensor, and one OLED display.

### Connections Used in the Prototype

| Component Pin | ESP32 Connection |
|---|---|
| DHT22 VCC | 3.3V |
| DHT22 DATA | GPIO 4 |
| DHT22 GND | GND |
| MQ-5 Analog Output | GPIO 34 through a suitable voltage divider |
| MQ-5 VCC | 5V |
| MQ-5 GND | GND |
| OLED VCC | 3.3V |
| OLED GND | GND |
| OLED SDA | GPIO 21 |
| OLED SCL | GPIO 22 |

A pull-up resistor can be connected between the DHT22 DATA pin and 3.3V. A voltage-divider circuit should be used between the MQ-5 analog output and ESP32 GPIO 34 where necessary, because the ESP32 analog input must not exceed 3.3V. Decoupling capacitors may be added across the supply lines to reduce noise and improve circuit stability.

### Architecture A Schematic

Place the Architecture A diagram in the `images` folder using this filename:

```text
images/architecture_a.png
```

Then display it in this document using:

```markdown
![Architecture A Schematic](images/architecture_a.png)
```

![Architecture A Schematic](images/architecture_a.png)

---

## 4.2 Architecture B

Architecture B will be added later. It will show one ESP32S connected to an MQ-5 sensor and interfaced directly with another ESP32S connected to a DHT22 sensor.

---

## 4.3 Architecture C

Architecture C will be added later. It will show one ESP32S connected to a DHT22 and relay module, interfaced with another ESP32S connected to an MQ-5 sensor.

---

# 5. Evidence of Group Work

Evidence of project work may include:

- GitHub commits
- Task allocation records
- Group communication screenshots
- Meeting screenshots
- Shared design or implementation discussions

At the moment, the submitted work contains the implementation and documentation completed by:

**William Githinji – 110592 – ICS 4B**

---

# Conclusion

The environmental requirements necessary for sunflower growth were identified and documented. Suitable hardware components were selected for monitoring temperature, humidity, soil moisture, soil pH, sunlight exposure and LPG gas levels. Datasheet links were provided for the major components. Architecture A was implemented and documented, while Architectures B and C will be completed in the next stage.
