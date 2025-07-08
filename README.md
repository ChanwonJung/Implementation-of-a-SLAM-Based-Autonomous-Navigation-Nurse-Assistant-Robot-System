# 🏥 Nursing Assistant Autonomous Robot System  

## 1. 📌 Project Overview

To address the excessive workload and burnout of nurses in hospital settings, we developed an autonomous robotic system that automates **medication delivery** and **vital sign monitoring**.

The system consists of **two TurtleBot4 robots** working cooperatively to perform logistics and patient interaction tasks across the **pharmacy and ward areas** in a hospital-like environment.

### System Architecture
<img width="920" alt="image" src="https://github.com/user-attachments/assets/9201e11e-0466-4b7a-8aae-bde2ca33f71c" />

### Node Architecture
<img width="1177" alt="image" src="https://github.com/user-attachments/assets/a5c84d87-49c2-4d37-9e85-74c5bc908902" />

### System flow
<img width="393" alt="image" src="https://github.com/user-attachments/assets/0e439a5b-1d56-4238-9ec0-7aecfa4f4423" />

---

## 2. ⚙️ Features and Functionalities

### ✅ Autonomous Navigation & Obstacle Avoidance
- SLAM-based navigation using ROS 2 Nav2
- Robust operation in complex environments like hospital corridors and rooms
- Dynamic obstacle detection (e.g. humans) with auto-stop and resume
  <img width="1208" alt="image" src="https://github.com/user-attachments/assets/78600910-01f6-47b8-b5a9-ef424c857cca" />


### ✅ Object and Patient Detection
- Real-time detection of medical items (Tylenol, bandages, etc.) using YOLOv8 and YOLOv11
- Patient identification using ArUco markers and face detection
- 3D localization via depth-based position estimation and TF2 transforms

### ✅ Contactless Vital Sign Monitoring
- rPPG-based estimation of heart rate, SpO2, and blood pressure
- Integrated with face tracking and signal enhancement filters

### ✅ Cloud-Based Robot Communication
- MQTT messaging over EMQX Cloud for stable multi-robot coordination
- Decentralized task assignment and rendezvous point logic

### ✅ Integrated GUI Control Panel
- Real-time logistics requests and monitoring
- Visual display of robot status, positions, and vital signs

---

## 3. 🧠 Tech Stack

| Category        | Technologies Used |
|----------------|-------------------|
| **Robot Platform** | TurtleBot4, ROS 2 Humble, Nav2 |
| **Vision System**  | OAK-D Camera, YOLOv8/YOLOv11, OpenCV |
| **Communication**  | MQTT, EMQX Cloud |
| **AI / Algorithms**| rPPG, Face Detection, KCF Tracker, CHROM, TF2 |
| **Development Env.** | Ubuntu 22.04, Python3, RViz2, Roboflow |
| **Collaboration** | GitHub, Google Docs, Presentation Tools |

<img width="727" alt="image" src="https://github.com/user-attachments/assets/82cc495a-b436-4a73-a29b-a479adc2bb34" />


---

## 4. 🌟 Outcomes & Impact

- Successfully demonstrated a full **autonomous robotic pipeline** for hospital logistics and patient interaction
- Integrated navigation, object recognition, face detection, and vital sign estimation into one real-time system
- Cloud-based structure ensures **scalability and reliability** for large-scale hospital deployment
- Enables nurses to focus on specialized medical tasks by **offloading repetitive labor**
- Provides a **foundational model for smart hospital infrastructure**

---

## 5. 🎥 Demo

- ▶️ [Demo Video] (https://drive.google.com/file/d/1XalQhJVQs6HRULGkdsYCedEdJGqS83Y0/view?usp=sharing)

---



