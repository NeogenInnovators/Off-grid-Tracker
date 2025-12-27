#  Off-Grid Tracker & Emergency Alert System!

The **Off-Grid Tracker System** is a wearable-based tracking and safety solution designed to **monitor people and transmit GPS data without relying on cellular networks, Wi-Fi, or internet services**. The system uses **LoRa communication**, **solar-powered towers**, and **wearable watches** to enable reliable tracking, emergency alerts, and identification in remote or disconnected environments.

This project is especially suitable for **disaster zones, remote areas, military regions, mines, forests, and off-grid industrial sites**.

**🎬Off-Grid Tracking System** (Google Drive Video):
 📁https://drive.google.com/file/d/1ISpZWWWw1rg_WSsy-IhYYVLMGUQDeksu/view?usp=drive_link

---



![IMG_20251226_150224](https://github.com/user-attachments/assets/6be466de-474c-4658-89f8-fd969934d335)


##  Objectives

* To develop an **internet-independent tracking and communication system** suitable for remote and mountainous regions.

* To ensure the **safety of trekkers and users** by continuously monitoring movement through **pole-based checkpoint tracking**.

* To assist in **disaster management scenarios**, such as floods, landslides, or other emergency situations.

* To provide a reliable **emergency SOS alert mechanism** through wearable devices and tracking poles.

* To enable **faster and more accurate rescue operations** by identifying the **last crossed checkpoint** and transmitting precise location data.

* To design a **scalable, cost-effective, and reliable solution** for outdoor tracking and safety applications.

---

##  Features of Smart Tracking Watch

*  **LoRa-Based Long-Range Communication:**
  Enables data transmission over long distances without the need for internet, Wi-Fi, or cellular networks.

*  **Integrated GPS Module:**
  Provides accurate location tracking by capturing real-time **latitude and longitude**, especially during emergency situations.

*  **Wearable & Lightweight Design:**
  Designed for comfort and ease of use, making it suitable for long-duration trekking and outdoor activities.

*  **NFC/RFID-Based User Identification:**
  Each watch contains a unique NFC/RFID tag to identify the user within the system.

*  **Checkpoint Interaction:**
  Automatically interacts with pole-based NFC readers to log checkpoint crossings.

*  **SOS Emergency Push Button:**
  Allows the user to instantly send an emergency alert in critical situations.

*  **Real-Time Data Transmission:**
  Sends movement data, SOS alerts, and GPS location information to the system in real time.

*  **Low Power Consumption:**
  Optimized for extended operation using battery power, ensuring long-lasting performance in off-grid environments.

---
##  Features of Tracking Pole (Tower)

* LoRa Communication:
Enables long-range, low-power wireless communication with the control panel without relying on cellular networks or Wi-Fi.

* Checkpoint-Based Installation:
Installed at regular intervals (approximately 5–10 km) to act as tracking and verification checkpoints along the route.

* NFC/RFID Reader Integration:
Identifies users by scanning the NFC/RFID tag embedded in the wearable watch when they pass a pole.

* Emergency SOS Push Button:
Allows users to manually trigger an emergency alert at the pole in critical situations.

* ESP32 Microcontroller:
Handles data processing, NFC/RFID scanning, and LoRa data transmission efficiently.

* Outdoor & Mountain-Ready Design:
Designed for reliable operation in harsh outdoor and mountainous environments.


---

##  Working of the System

The Off-Grid Tracker & Emergency Alert System operates through coordinated interaction between the control panel, tracking poles, and smart tracking watches. The system enables continuous monitoring, checkpoint-based tracking, and emergency response without relying on the internet or mobile networks.

---

### **1. Control Panel**
![IMG_20251226_140911](https://github.com/user-attachments/assets/864a334e-f75f-4b8f-9752-fff1ab3fa4bc)


The Control Panel acts as the **central monitoring and decision-making unit** of the system.

**Components:**

* **ESP32:** Main processing and control unit
* **LoRa Module:** Long-range communication with poles and watches
* **OLED Display:** Real-time status and alert visualization

**Functions:**

* Receives data from tracking poles and smart watches
* Displays the **last crossed pole** for each user
* Shows **SOS alerts along with exact GPS coordinates (latitude & longitude)**
* Monitors user movement, progress, and system status in real time

---

### **2. Tracking Poles**

![IMG_20251226_141116](https://github.com/user-attachments/assets/235da4c8-2933-4b5a-b33b-797cc61bf1c7)
![IMG_20251226_141259](https://github.com/user-attachments/assets/dac278dc-1e44-4142-9618-3a7636cd84d2)

Tracking poles serve as **checkpoint units**, installed at regular intervals (approximately **5–10 km**) along the route.

**Components:**

* **ESP32:** Data processing and control
* **LoRa Module:** Communication with the control panel
* **NFC/RFID Reader:** User identification via watch
* **SOS Push Button:** Manual emergency alert trigger

**Functions:**

* Detect users when they reach a checkpoint using NFC/RFID scanning
* Forward **User ID, Pole ID, and Timestamp** to the control panel
* Allow users to trigger an SOS alert directly from the pole if required

---

### **3. Smart Tracking Watch**

Each user is provided with a smart tracking watch for **personal safety and location tracking**.

**Components:**

* **Arduino Nano:** Processing unit
* **LoRa Module:** Long-range data transmission
* **NFC/RFID Tag:** Unique user identification
* **GPS Module:** Accurate location tracking
* **SOS Push Button:** Emergency alert

**Functions:**

* User taps the watch near a pole to log checkpoint crossing
* Watch transmits **user ID and real-time GPS location** to the nearest pole via LoRa
* The pole forwards this data to the control panel
* In emergencies, pressing the SOS button sends an **instant alert with GPS coordinates**

---

### **4. Real-Time Tracking & Monitoring**

The system continuously updates and displays:

* User location and route progress
* Last crossed checkpoint
* Active SOS alerts with GPS coordinates

This enables quick identification of missing users and ensures that trekkers remain on the correct route.

---

### **5. Emergency Handling**

**SOS Alert Flow:**

1. User presses the SOS button on the watch or at a tracking pole
2. The LoRa module transmits the SOS alert along with GPS location data
3. The control panel receives and displays the alert
4. Rescue teams are notified with the **exact last known location**

### **6. Internet-Independent Operation**

* The entire system operates **without internet, Wi-Fi, or mobile networks**
* **LoRa technology** enables long-range, low-power communication
* Suitable for **remote, mountainous, and disaster-prone environments**

---

## *Future enhancement:* Drones may be deployed to deliver medical supplies or emergency equipment to the user’s location.(WORKING ON DRONE ALSO)
📁VIDEO ATTACHED:https://drive.google.com/file/d/1dyMqwY5t-to7OFGztk3n1JHkRVxIuUXC/view?usp=sharing
---

##  System Flowchart (Operational Workflow)

![zaid](https://github.com/user-attachments/assets/6d1ebb05-a6aa-4f37-b3a9-59b69cce613a)

---

##  Data Flow Diagram (DFD)

The Data Flow Diagram (DFD) represents how data moves through the Off-Grid Tracker & Emergency Alert System, from the user to the rescue authorities. It highlights the interaction between the wearable watch, tracking poles, communication layer, and control panel in an off-grid environment.



![WhatsApp Image 2025-12-27 at 5 57 33 PM](https://github.com/user-attachments/assets/8c5c94e0-b22a-4090-9601-f7ffd02d10d8)

---

###  DFD – Explanation

* **User:**
  The user wears the smart tracking watch and can trigger an SOS alert when needed.

* **Smart Tracking Watch:**
  Collects GPS coordinates, holds the NFC/RFID-based unique ID, and sends user data or SOS alerts using LoRa communication.

* **Pole Checkpoint:**
  Acts as a checkpoint that scans the NFC/RFID tag from the watch and forwards user data along with pole ID and timestamp.

* **LoRa Communication Layer:**
  Enables long-range, low-power, internet-independent data transfer between system components.

* **Control Panel:**
  Receives and analyzes incoming data, displays real-time user status, GPS coordinates, and alerts on the OLED screen.

* **Emergency Decision Module:**
  Validates SOS alerts, identifies the last crossed pole, and prepares actionable information.

* **Rescue Team / Authorities:**
  Receive verified emergency information to initiate fast and accurate rescue operations.

---

##  Challenges


*  **Power Supply in Remote Areas**
  Ensuring uninterrupted power for poles, control panels, and wearable devices is challenging. Solar-powered systems are highly dependent on weather conditions such as limited sunlight, rain, or snow.


*  **Hardware Dependency and Reliability**
  The system relies on multiple hardware components such as ESP32, Arduino Nano, LoRa modules, GPS modules, and NFC readers. Failure of any single component can impact overall system performance.

*  **Device Durability in Extreme Conditions**
  Poles and wearable devices must withstand harsh environmental conditions including rain, snow, dust, extreme temperatures, and physical impact, which increases design and maintenance complexity.


*  **Environmental Interference with LoRa Signals**
  Natural obstacles, atmospheric conditions, and electromagnetic interference may degrade LoRa signal quality, affecting data transmission reliability.

---

##✔️  **ROUND 1 FEATURES COMPLETED**


* **1.SIGNAL COVERAGE – Up to 10 km**

  Long-range LoRa communication enables reliable data transmission up to 10 km without internet or cellular networks, making the system ideal for remote and off-grid environments.

* **2.SOS Message Transmission & Reception**

  Users can trigger SOS alerts from the smart watch or tracking pole. The control panel instantly receives the alert along with precise GPS coordinates, enabling fast emergency response.

* **3.Microcontroller Fully Working**

  The system uses **ESP32** in poles and the control panel, and **Arduino Nano** in smart watches, ensuring efficient processing of GPS data, LoRa communication, checkpoint logging, and emergency alerts with low power consumption.

* **4.Checkpoints installed**

  Tracking poles act as checkpints where users tap their NFC-enabled watches. This logs user position and movement, ensuring accurate route monitoring and improved safety tracking.

---

##**⏭️ ROUND 2 EXPECTED IMPROVEMENTS**


### **1. GPS Location Integration**

Each smart tracking watch is equipped with an integrated GPS module that provides accurate real-time location data. During emergency situations, when the user presses the SOS button, the watch transmits precise GPS coordinates (latitude and longitude) to the control panel, enabling rescue teams to locate and assist the user quickly and accurately.


### **2. Extended LoRa Communication Range (Up to 15 km)**

The system uses LoRa for long-range, low-power communication between watches, poles, and the control panel, with an effective range of up to **15 km**.

If a user moves beyond the LoRa coverage area:

* The smart watch stores checkpoint and SOS data locally.
* Once the user re-enters the communication range, the stored data is automatically transmitted to the nearest pole and then forwarded to the control panel.

This improvement ensures **reliable data delivery and zero data loss**, even in extremely remote locations.


### **3. NFC-Based User Identification**

Each smart tracking watch contains a unique NFC tag for secure and accurate user identification. When the user taps the watch on a tracking pole:

* The pole reads the NFC tag.
* The user ID along with checkpoint information is transmitted to the control panel.

This feature prevents user misidentification and ensures precise tracking when multiple users are present on the same route.

##  PredIcted  Improvements (FUTURISTIC SCOPE)
![IMG_20251226_150210](https://github.com/user-attachments/assets/db47d8ca-408d-40bc-9024-9a7fae1f4fe1)

*  **Mobile App Dashboard**
  Develop a mobile application to visualize real-time GPS locations of users on an interactive map (e.g., Google Maps). This will make tracking, monitoring, and emergency response more intuitive and accessible.

*  **Cloud Integration**
  Integrate cloud platforms to store tracking data, SOS alerts, and user information. This will enable remote system access, advanced analytics, and historical data management for improved decision-making.

*  **Drone Assistance for Emergencies**
  Deploy drones to deliver medical supplies, communication devices, or emergency materials to users in distress, significantly reducing response time during critical situations.

*  **Enhanced Solar-Powered Devices**
  Further integrate and optimize solar panels for both poles and wearable devices to ensure a sustainable and uninterrupted power supply in remote locations, minimizing reliance on conventional batteries.

---


##  Team

* **Team Name:** *Neogen Innovators*
* **Members:** 

    *Sumaira*

    *Shiny*

    *Mohd Zaid Anasri*

    *Nevid Alam*
    
* **Hackathon:** *HACK THE WINTER(THE SECOND WAVE)*

---


