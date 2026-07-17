# ICS 4111 – Embedded Systems & IoT

# Semester Project – Deliverable 3

## Student Details

**Name:** William Githinji  
**Admission Number:** 110592  
**Class:** ICS 4B  

**Project Title:** Sunflower Environmental Monitoring System

---

# 1. Objective

The objective of this deliverable was to transmit environmental sensor data from an ESP32-based embedded system to cloud platforms for storage and visualization using InfluxDB Cloud and Grafana.

---

# 2. Prototype Description

A simulated prototype based on Architecture A was developed using Wokwi.

The prototype consists of:

- ESP32 DevKit
- DHT22 Temperature and Humidity Sensor
- MQ-5 Gas Sensor (simulated)
- OLED Display
- Wi-Fi Connectivity

The ESP32 reads sensor data, displays the readings on the OLED display, and transmits the information to InfluxDB Cloud over Wi-Fi.

---

# 3. Wokwi Simulation

**Public Wokwi Project**

https://wokwi.com/projects/469817118769556481

---

# 4. Cloud Data Storage

InfluxDB Cloud was used as the time-series database.

The ESP32 transmitted:

- Temperature readings
- Humidity readings
- Gas sensor readings

The data was successfully stored as time-series records for later visualization.

---

# 5. Grafana Dashboard

Grafana was connected to the InfluxDB Cloud database.

The dashboard visualized the collected sensor data using multiple charts.

The dashboard includes:

- Temperature visualization
- Humidity visualization
- Gas sensor visualization

---

# 6. System Workflow

1. ESP32 collects sensor readings.
2. Sensor values are displayed on the OLED display.
3. ESP32 connects to Wi-Fi.
4. Sensor readings are transmitted to InfluxDB Cloud.
5. InfluxDB stores the readings as time-series data.
6. Grafana retrieves the stored data and displays it on dashboards.

---

# 7. Physical Prototype Status

The physical implementation was not completed before submission.

The complete functionality of the system was successfully demonstrated using the Wokwi simulation environment together with InfluxDB Cloud and Grafana.

---

# 8. Challenges Encountered

The physical prototype was not assembled before submission.

The simulation platform was therefore used to validate the complete system, including cloud communication and dashboard visualization.


---

# Conclusion

The objective of transmitting environmental sensor data to cloud platforms was successfully achieved using a simulated ESP32 prototype. Sensor readings were transmitted to InfluxDB Cloud, stored as time-series data, and visualized through Grafana dashboards. The project demonstrates a complete IoT data pipeline from sensing to cloud visualization.
