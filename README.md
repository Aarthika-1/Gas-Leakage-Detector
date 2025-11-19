# Gas-Leakage-Detector
📊 System Flowchart
Start
   ↓
Read gas sensor value
   ↓
Is gas > threshold?
   ├── Yes → Activate alarm (Buzzer + LED)
   └── No  → Safe mode (Green LED)
   ↓
Repeat

🔧 Circuit Diagram (Description)

MQ sensor AO pin → A0 of microcontroller

Buzzer → Digital Pin 8

Red LED → Pin 9 (with resistor)

Green LED → Pin 10

VCC & GND → Power supply

(Users can add their Fritzing diagram here.)

📱 Optional: IoT Notifications

You can integrate this with:

Blynk App (via WiFi module)

MQTT + Node-RED

ThingSpeak

This enables SMS/push notifications for gas leakage.

🧪 Testing Procedure

Power the system

Check baseline value on Serial Monitor

Bring a small amount of LPG near the sensor (DO NOT use open flames)

Observe value rise → alarm triggers

📌 Applications

Household kitchens

Hotels and restaurants

Gas storage rooms

Laboratories

Industrial environments
