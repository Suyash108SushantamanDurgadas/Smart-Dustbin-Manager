# Smart Dustbin Manager (ESP32)

This project is an **ESP32-based smart dustbin** that uses ultrasonic sensors and a servo-based radar sweep to measure waste fill levels. It features:
- **Radar sweep calculation** for accurate area-based fill level estimation.
- **State Machine (FSM)** with `MONITORING`, `PROCESSING`, and `SHUTDOWN` modes.
- **Manual Reset** using a button when the bin is serviced.
- **Servo-controlled lid** for user detection.

---

## Hardware Used
- ESP32 Dev Board  
- Ultrasonic Sensors (HC-SR04) ×3  
- Servo Motors ×2  
- Push Button  

---

## Working
1. **Monitoring**: Detects users and opens/closes the lid.
2. **Processing**: Performs radar sweep to calculate fill percentage.
3. **Shutdown**: Locks when fill ≥80%. Requires manual button press to recheck.

---

## How to Use
1. Upload `smart_dustbin.ino` to ESP32.  
2. Connect hardware as per pin definitions.  
3. Open Serial Monitor at 115200 baud for status logs.

---

## Simulation
[Wokwi Project Link](#) *(Add your Wokwi link here)*  

---

## Future Work
- IoT integration with Blynk or Firebase for remote monitoring.
- Automated SMS/Email alerts on bin full.
