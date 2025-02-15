🔧 Components Required:
1️⃣ Microcontroller:
Arduino (Pro Mini, Uno, or Nano) → The brain of the system
2️⃣ Sensors:
HC-SR04 Ultrasonic Sensor → Measures the distance of an object
Soil Moisture Sensor (Analog) → Determines moisture content (used to detect wet waste)
3️⃣ Actuators:
Servo Motor (SG90 / MG995) → Moves to direct wet or dry waste into the correct bin
4️⃣ Power & Connections:
Power Source (5V) → USB adapter, LiPo battery, or a 9V battery with a voltage regulator
Jumper Wires → For making connections
📌 Working Principle:
Waste Detection:

The ultrasonic sensor (HC-SR04) continuously checks for objects (waste items).
If an object is detected within 15 cm, the system proceeds to moisture analysis.
Moisture Measurement:

The soil moisture sensor measures the waste's moisture level.
If moisture content > threshold (e.g., 1 in the code), it's classified as wet waste.
If moisture content ≤ threshold, it's classified as dry waste.
Waste Sorting Using Servo Motor:

Wet waste: The servo motor moves to 170°, directing the item to the wet bin.
Dry waste: The servo motor moves to 10°, directing the item to the dry bin.
After sorting, the servo resets to 90° for the next waste item.
Serial Monitor Output:

The humidity percentage and distance are displayed in the Serial Monitor.
It also prints whether the detected waste is wet or dry.
🔗 Connections:
1️⃣ Ultrasonic Sensor (HC-SR04) to Arduino
HC-SR04 Pin	Arduino Pin
VCC	5V
GND	GND
Trig	D12
Echo	D11
2️⃣ Soil Moisture Sensor to Arduino
Soil Sensor Pin	Arduino Pin
VCC	5V
GND	GND
Analog OUT	A0
3️⃣ Servo Motor to Arduino
Servo Pin	Arduino Pin
VCC	5V
GND	GND
Signal	D8
🚀 Project Applications:
✅ Smart Waste Management in homes, offices, and public places
✅ Automation in waste segregation plants
✅ Educational Projects for learning Arduino and sensors
