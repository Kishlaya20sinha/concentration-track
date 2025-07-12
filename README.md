# 🧠✨ Concentration Tracker: An AI-Powered Attentiveness System

**Author:** Kishlaya Sinha  
📧 Email: [kishlaya20sinha@gmail.com](mailto:kishlaya20sinha@gmail.com)  
🔗 GitHub: [Kishlaya20sinha](https://github.com/Kishlaya20sinha)  
💼 LinkedIn: [Kishlaya Sinha](https://www.linkedin.com/in/kishlaya-sinha-9134a0211/)

---

## 🚀 Overview

This project presents the **Concentration Tracker**, a cutting-edge real-time system designed to monitor and evaluate user attentiveness.  
By integrating **MediaPipe** and **OpenCV**, it analyzes physiological indicators like eye blinks, gaze direction, and head pose.

Ideal for:
- Academic environments 📚
- E-learning platforms 🧑‍💻
- Workplace productivity tools 📈

It provides immediate visual feedback to help users manage their focus effectively.

---

## 🎯 Core Functionalities

- **Ocular Blink Detection 👀**  
  Uses Eye Aspect Ratio (EAR) to detect blinks and closed-eye durations.

- **Gaze Direction Analysis ➡️**  
  Analyzes iris landmarks to determine attention direction.

- **Head Pose Estimation 🧑‍🦰**  
  Uses nose position to infer head orientation.

- **Integrated Concentration Metric 📊**  
  Combines blink, gaze, and head pose into a concentration score.

- **Dynamic Visual Feedback 📺**  
  Live webcam overlay showing focus level, blink alerts, and distraction counts.

- **Distraction Monitoring 🚫**  
  Tracks inattention over time and triggers alerts.

---

## 🖼️ Illustrative Output

The live webcam feed displays:
- 💯 Concentration percentage
- 👁️‍🗨️ Real-time blink alerts
- 🔢 Distraction counter
- ✅❌ "ACTIVE" or "DISTRACTED" status
- ⚡ FPS for performance monitoring

---

## 💻 Technological Framework

- **Python 3.x** 🐍
- **OpenCV** 📸
- **MediaPipe (FaceMesh)** ✨
- **NumPy** ➕

---

## ⚙️ Operational Methodology

1. **Facial Landmark Detection 📍**  
   Uses MediaPipe FaceMesh for key facial features.

2. **Blink Recognition 👁️**  
   Calculates EAR to identify blink events.

3. **Gaze Analysis ➡️**  
   Analyzes iris position for gaze direction.

4. **Head Pose Inference 🧭**  
   Uses nose coordinates to infer orientation.

5. **Concentration Score Calculation 🧮**  
   Combines metrics with weighted formula:

   ```text
   Concentration Score = 0.4 × gaze + 0.4 × head_pose + 0.2 × absence_of_blinking

6. **Live Interface Rendering 🖥️**
   Displays real-time concentration feedback on screen.

## Run the Project

```bash
git clone https://github.com/Kishlaya20sinha/concentration-track.git
cd concentration-tracker
pip install -r requirements.txt
python concentration_tracker.py
