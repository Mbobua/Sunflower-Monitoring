# ICS 4111 – Embedded Systems & IoT

# Semester Project – Deliverable 2

## Student Details

**Name:** William Githinji  
**Admission Number:** 110592  
**Class:** ICS 4B  

**Project Title:** Sunflower Environmental Monitoring System

---

# 1. Objective

The objective of this deliverable was to develop and test embedded system prototypes based on the architectures designed in Deliverable 1. Architecture A was successfully implemented and tested using the Wokwi simulation platform.

---

# 2. Prototype Overview

Architecture A consists of:

- ESP32 DevKit
- DHT22 Temperature and Humidity Sensor
- MQ-5 Gas Sensor (simulated)
- OLED Display
- Wi-Fi Connectivity
- InfluxDB Cloud
- Grafana Dashboard

The ESP32 collects sensor readings, displays them on the OLED display and transmits the data to InfluxDB Cloud for visualization in Grafana.

---

# 3. Wokwi Simulation

The simulated prototype was successfully implemented using Wokwi.

**Public Wokwi Project**

https://wokwi.com/projects/469817118769556481

---

# 4. Prototype Functionality

The prototype successfully performs the following tasks:

- Reads temperature values.
- Reads humidity values.
- Reads gas sensor values.
- Displays sensor readings on the OLED display.
- Sends sensor data to InfluxDB Cloud.
- Visualizes sensor data using Grafana dashboards.

---

# 5. Simulation Results

The simulation demonstrated successful communication between all components. Sensor readings were displayed correctly on the OLED display and transmitted to InfluxDB Cloud, where they were visualized using Grafana.

---

# 6. Physical Prototype Status

The physical implementation of Architecture A was not completed before submission.

However, the simulated prototype was successfully developed and tested using Wokwi. The simulation demonstrated the intended functionality of the system, including sensor data acquisition, OLED display output, and transmission of data to InfluxDB Cloud for visualization in Grafana.

---

# 7. Challenges Encountered

I was unable to assemble and test the physical prototype before submission. As a result, only the simulated prototype is presented in this deliverable.

---

# 8. Solutions Explored

- Successfully developed and tested the complete system using Wokwi.
- Verified sensor readings through the Serial Monitor.
- Verified OLED display output.
- Successfully connected the ESP32 to InfluxDB Cloud.
- Successfully visualized sensor data using Grafana.

---

# 9. Future Work

- Assemble and test the physical prototype.
- Implement Architecture B.
- Implement Architecture C.
- Compare physical prototype results with simulation results.

---

# 10. Evidence of Group Work

Evidence may include:

- GitHub commits
- Team discussions
- Task allocation
- Meeting records

---

# Conclusion

Architecture A was successfully implemented and tested in the Wokwi simulation environment. The simulation confirmed correct operation of the embedded system and successful cloud integration using InfluxDB and Grafana. The physical implementation and the remaining architectures will be completed in subsequent stages of the project.
