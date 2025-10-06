# 💧 Lab 01: Real-time Data Acquisition and Visualization with a Water Level Sensor

This lab demonstrates **real-time water level monitoring**, **data processing**, and **visualization** using an Arduino-compatible water level sensor.  
It includes tasks for sensor interfacing, data mapping, threshold-based alarms, and rate-of-change computation — with an optional buzzer for high-level alerts.

---

## 🧩 Part 1: Sensor Interfacing and Initial Reading
**Code:** [`sketch_oct6b.ino`](sketch_oct6b.ino)

- Connects the **analog water level sensor** to the Arduino.  
- Reads raw sensor values (0–1023) and prints them to the **Serial Monitor** for initial calibration.

---

## ⚙️ Part 2: Programming and Data Processing Tasks
**Code:** [`sketch_oct6c.ino`](sketch_oct6c.ino)

### 🧮 Task 1: Data Mapping and Visualization
- Maps the **raw sensor values** (0–1023) to a **percentage scale (0–100%)** using the `map()` function.  
- Displays both raw and mapped data in the **Serial Plotter** for real-time visualization.  

### 🚨 Task 2: Water Level Alarms
- Defines threshold levels:
  - **LOW LEVEL:** 25%  
  - **MEDIUM LEVEL:** 75%  
  - **HIGH LEVEL:** 95%  
- Uses conditional checks (`if-else`) to print specific alerts when levels change.  
- Visualizes data while showing alerts in the **Serial Monitor**.

### 📈 Task 3: Calculate and Plot Rate of Change
- Computes how quickly the water level is **rising or falling**.  
- Calculates the **rate of change** as the difference between consecutive readings.  
- Prints both **current percentage** and **rate of change** for simultaneous visualization in the **Serial Plotter**.

---

## 🔔 Extra Part: Buzzer for High-Level Alert
**Code:** [`sketch_oct6e.ino`](sketch_oct6e.ino)

- Adds an **audible buzzer** that triggers **only when the water level exceeds 95%**.  
- Enhances real-time alerting for overflow conditions.  
---

## 🧠 Summary
| Feature | Description |
|----------|--------------|
| **Sensor** | Analog water level sensor connected to Arduino |
| **Visualization** | Serial Plotter shows real-time percentage & rate of change |
| **Alerts** | Text-based alerts for low/medium/high levels |
| **Audio Alarm** | Buzzer sounds when water level > 95% |
| **LED Indicator** | Turns ON for medium & high levels |

---

### 🛠️ Hardware Requirements
- Arduino UNO (or compatible board)  
- Water level sensor (analog output)  
- Buzzer  
- Jumper wires  
- USB cable  

---

### 📊 Output Visualization
- **Serial Monitor:** Displays alert messages  
- **Serial Plotter:** Shows two lines — *water level percentage* and *rate of change*  

---

### 👨‍💻 Author
**Suddip Paul Arnab**  
*Department of Computer Science & Engineering*  
*East West University*

---

