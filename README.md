# Projects
Project Name : Dynamic Spectrum Allocation using Priority Queue
# A real-time two-way communication system for emergency rescue, using ESP32, C, and Wi-Fi—no internet needed.
Problem Solved
In disaster-prone or remote areas with no internet, this project enables victims to send help requests to rescue teams over a local Wi-Fi network hosted by ESP32.

# Features
- ESP32 acts as a hotspot server (no internet needed)
- Hosts a webpage that shows:
  - Name
  - Age
  - "Help" trigger button
- When “Help” is clicked:
  - A buzzer sounds on the receiver end
  - Victim info is logged using priority queue logic
- SSID / RSSI values used to prioritize requests (e.g., signal strength = proximity)
- Lightweight C implementation on ESP32 with Web UI
  
 # Tech Stack
-  ESP32 (Wi-Fi hotspot & web server)
-  C programming (priority queue logic)
-  RSSI/SSID-based signal detection
-  HTML/CSS for the local web interface
-  Buzzer for physical alerts
  
# How It Works
1. ESP32 creates a local Wi-Fi hotspot
2. Victim connects phone and opens hosted webpage
3. Fills Name, Age, and hits "Help"
4. ESP32 receives data, prioritizes it using signal strength
5. Sends buzzer signal to alert rescue team
6. Two-way communication possible if ESP32 acts as relay
