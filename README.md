# 🚦 Traffic Signal Synchronization and Dynamic Control

> A smart traffic management system powered by **IoT, real-time sensors, and embedded systems** to optimize urban mobility.  
> Developed as a final-year engineering project at **D.Y. Patil College of Engineering & Technology, Kolhapur**, and **published in IJRASET (Oct 2023)**.

[![DOI](https://img.shields.io/badge/Published-IJRASET-blue)](https://doi.org/10.22214/ijraset.2023.56156)
![IoT](https://img.shields.io/badge/built%20with-IoT%20%7C%20Arduino-green)
![SmartCity](https://img.shields.io/badge/focus-Smart%20Cities-blue)
![Real-Time](https://img.shields.io/badge/data%20flow-Real%20Time-yellow)

---

## 📌 About the Project

Modern cities are evolving — but unplanned traffic intersections still cause **congestion, delays, and safety issues**. This project proposes a **real-time, sensor-driven synchronization model** for traffic lights that adapts based on live vehicle density using **IR sensors and Arduino**.

Built as a **smart city solution**, the system clusters nearby intersections and dynamically allocates green light time to lanes with the most traffic — improving flow and reducing wait times.

---

## 🎯 Objectives

- 🔁 Synchronize 2–3 traffic lights dynamically in dense urban clusters
- 📡 Use **infrared sensors (IRS1, IRS2)** to detect traffic volume per lane
- 🧠 Prioritize high-traffic lanes in real-time
- 📲 Integrate with a **mobile app and maps** for real-time signal status
- 🌙 Adapt behavior for **night mode** to reduce power usage and accidents

---

## 💡 Why It Matters

✅ Real-time congestion management  
✅ Safer night intersections (auto-detect vehicles → green light)  
✅ Better signal utilization = fewer unnecessary stops  
✅ Potential for integration into **Google Maps & surveillance systems**  
✅ Scalable to smart cities & developing urban areas

---

## 🔍 How It Works

- Each **lane** has 2 infrared sensors (placed 50m apart)
- If both detect vehicles → higher lane density is inferred
- Green light duration is extended proportionally
- Signals of adjacent intersections are then synchronized accordingly
- At night, signal stays red unless IRS1 detects a vehicle (prevents speeding)

---

## 🛠️ Tech Stack & Tools

| Component           | Technology                         |
|--------------------|-------------------------------------|
| Embedded Controller | **Arduino UNO**                    |
| Sensors             | **IR Sensor (IRS1, IRS2)**         |
| Connectivity        | Wi-Fi Module (for mobile sync)     |
| Mobile Integration  | Android App (real-time signal view)|
| Programming         | C++ (Arduino IDE), XML (UI)        |
| Architecture        | IoT + Edge Computing               |

---

## 📱 Real-Time Mobile Companion

- Displays current signal color at each connected intersection
- Option to embed in navigation apps like Google Maps
- Useful for emergency vehicles and route planning

---

## 🧪 Field Example: Cluster-Based Synchronization

```plaintext
Cluster: 3 Intersections (A, B, C)
Intersection A has highest traffic → given 45 sec green
Intersections B & C adjust timing to match Intersection A

Result:
↳ Fewer lane changes
↳ Smoother traffic flow across junctions
↳ Lower accident risks
