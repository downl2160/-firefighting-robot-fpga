# Project Summary

**Problem Statement**  
Fire accidents endanger lives, property, and the environment, especially in areas that are hard to reach or too hazardous for human firefighters. Traditional firefighting methods can be slow to respond and put responders at risk.

**Objectives**  
- Design an autonomous, mobile platform capable of detecting and extinguishing indoor fires without human intervention.  
- Improve response time and safety by using multi-sensor fusion and AI confirmation to avoid false positives.  
- Implement user notifications and emergency alerts when a fire is detected.  
- Demonstrate viability in a lab environment with working prototypes that can:  
  - Navigate obstacles  
  - Confirm fire presence (95%+ accuracy)  
  - Target and extinguish flames with a high-pressure nozzle  
  - Notify the user via Blynk app and email  
  - Automatically place a call to the local fire department (Prototype-2)  
  - Provide remote monitoring via IoT  

**Approach**  
1. **Hardware Integration**  
   - Caterpillar-track chassis with shock-absorbing front wheels  
   - Master–Slave Arduino network for distributed control  
   - Multi-sensor array (flame, smoke, PIR, ultrasonic, temperature/humidity, UWB radar, infrared camera)  
   - 2 HP centrifugal pump and 2-axis servo nozzle  

2. **AI & FPGA**  
   - Trained a CNN on infrared-camera frames and additional sensor data to confirm real fires  
   - Deployed inference on a custom FPGA for millisecond-scale decision making  

3. **Software & IoT**  
   - Real-time sensor fusion and motor control via Arduino code  
   - Remote telemetry and manual override through Blynk on ESP8266 modules  
   - Email API integration for alert messages  
   - GSM/VoIP module integration (Prototype-2) to auto dial fire department  

**Impact**  
- Rapid, reliable fire detection and suppression in challenging indoor environments  
- Immediate emergency alerts reduce response time by notifying both users and fire services  
- Minimization of firefighter exposure to danger  
- Foundation for future enhancements, including autonomous mapping and full human-detection  
