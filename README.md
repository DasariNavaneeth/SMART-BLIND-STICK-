#  Smart Blind Stick for Visually Impaired Individuals  
---
##  Overview  

The **Smart Blind Stick** is an assistive device designed to help visually impaired individuals navigate safely.  
It integrates multiple sensors to detect obstacles, measure depth, detect falls, and send GPS location alerts to family members via **Twilio SMS**.  
The stick provides real-time feedback through a **buzzer**, ensuring both safety and independence.  

---

##  Components Used  

- Raspberry Pi Pico  
- GPS Module  
- Ultrasonic Sensors (x2)  
- Gyroscope Sensor  
- Buzzer  
- Push Button  
- Resistors (as needed)  
- Breadboard / PCB  
- 9V Battery  

---

##  Features  

### 🔹 Obstacle Detection  
- Ultrasonic sensor detects nearby obstacles and alerts the user through a buzzer.  

### 🔹 Depth Detection  
- Another ultrasonic sensor measures the depth of drop-offs or steps to prevent falls.  

### 🔹 Fall Detection with Delay  
- The gyroscope detects if the user falls.  
- After a **10-second delay**, the GPS module sends the user’s location to family members via **Twilio SMS**.  
- The delay allows the user to cancel **false alarms**.  

### 🔹 Manual Location Alert  
- Pressing the **push button** sends the user’s GPS location immediately via **Twilio SMS**.  

### 🔹 GPS Fallback via IP  
- If GPS fails to get a fix, the system uses **IP-based geolocation** to fetch an approximate location and send it via Twilio SMS.  

### 🔹 Buzzer Alerts  
- Different **beep patterns** indicate:
  - Depth detection  
  - Obstacle detection  

---

##  Applications  

- Navigation assistance for visually impaired individuals  
- Safety enhancement during walking or mobility  
- Prototype for wearable assistive technology  

---

##  Programming Language  

- **MicroPython** (for Raspberry Pi Pico)  

---

##  Future Improvements  

- Add **voice feedback** using a speaker module  
- Integrate **Bluetooth** or **Wi-Fi** tracking for live monitoring  
- Use **rechargeable Li-ion battery** for portable
  
