# ✋ Hand Detection Interface – Milestone 1

## 📌 Project Overview
The **Hand Detection Interface** is a computer vision application built using **Streamlit, OpenCV, and MediaPipe**. This milestone focuses on detecting human hands from a webcam feed and displaying real-time detection information through an interactive web interface.

The system captures live video, processes frames using the **MediaPipe Hand Tracking model**, and visualizes detected hand landmarks and connections. It also provides performance metrics such as **FPS, number of hands detected, landmarks, and detection status**.

This milestone serves as the **foundation for gesture-based interaction systems**, which can later be extended for applications like **gesture-controlled volume systems, touchless interfaces, and assistive technologies**.

---

# 🎯 Objectives
- Develop a **real-time hand detection system**
- Capture video using the **system webcam**
- Detect **hand landmarks using MediaPipe**
- Display results in a **Streamlit web interface**
- Show **detection metrics and status updates**
- Provide controls to **start, stop, and capture frames**

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming language |
| Streamlit | Interactive web interface |
| OpenCV | Video capture and image processing |
| MediaPipe | Hand detection and landmark tracking |
| HTML/CSS | Interface styling |

---

# 📂 Project Structure

```
HAND_GESTURE_MILESTONE1
│
├── milestone1.py
├── captured_frame.png   # Captured image (generated after capture)
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/akhilakummari-26/HAND_GESTURE_MILESTONE_1.git
```

---

## 2️⃣ Install Dependencies

Install the below libraries:

```bash
pip install streamlit opencv-python mediapipe
```

---

# ▶️ Running the Application

Run the Streamlit application using:

```bash
streamlit run milestone1.py
```

The application will open in your browser at:

```
http://localhost:8501
```

---

# 🖥️ Application Interface

The application consists of two main sections.

### Left Panel
- Displays **live webcam feed**
- Shows **hand landmark visualization**
- Updates in real-time

### Right Panel

Displays detection information including:

#### Detection Status
- Camera Status
- Hands Detected
- Detection FPS
- Model Status

#### Detection Parameters
- Detection Confidence
- Tracking Confidence
- Maximum Number of Hands

#### Detection Info Cards
- Number of Landmarks
- Number of Connections
- Camera Resolution
- Detection Latency

---

# 🎮 Controls

| Button | Function |
|------|------|
| Start Camera | Starts the webcam |
| Stop Camera | Stops the webcam |
| Capture | Saves the current frame |

Captured images are stored as:

```
captured_frame.png
```

---

# 🧠 How Hand Detection Works

1. The webcam captures frames using **OpenCV**.
2. Frames are converted from **BGR to RGB format**.
3. The **MediaPipe Hands model** processes the frame.
4. The model detects **21 landmarks per hand**.
5. Landmarks and connections are drawn on the frame.
6. Detection metrics such as **FPS and hand count** are displayed.

---

# 📊 Hand Landmark Model

The MediaPipe Hands model detects **21 key points** on each hand including:

- Wrist
- Thumb joints
- Index finger joints
- Middle finger joints
- Ring finger joints
- Little finger joints

These landmarks allow accurate **gesture recognition and tracking**.

---

# 🚀 Future Improvements

Future milestones may include:

- Gesture recognition
- Volume control using hand gestures
- Finger distance measurement
- AI gesture classification
- Smart touchless interfaces

---

# 📚 Applications

This technology can be used in:

- Smart home systems
- Touchless user interfaces
- Gaming systems
- Virtual reality applications
- Assistive technologies
- Human-computer interaction

---

# 👩‍💻 Author

**Akhila Kummari**

---

# 📜 License

This project is licensed under the MIT License.
