# 🪑 Smart Chair 
This project introduces an innovative **hand gesture-controlled smart chair** that uses a **Raspberry Pi 4**, **OpenCV**, and **Python** to interpret user gestures for motor-based movement. It's a fusion of **computer vision**, **GPIO control**, and **embedded systems** designed for smart environments and accessibility support.

---

## 📌 Features

- ✋ Real-time hand gesture recognition using OpenCV
- ⚙️ Motor control via GPIO pins on Raspberry Pi
- 📷 Live camera feed for interaction
- 🔌 Custom Raspberry Pi OS image with all dependencies pre-installed
- 📁 Python-based modular code

---

## 🎯 Project Objectives

- Implement gesture recognition to control chair movement (e.g., forward, backward, left, right).
- Interface Raspberry Pi GPIO pins with motor drivers.
- Achieve smooth, reliable operation for accessibility or smart furniture purposes.

---

## 🛠️ Hardware Requirements

| Component             | Details                                |
|----------------------|----------------------------------------|
| Raspberry Pi         | Version 4 (with Raspbian OS)           |
| Camera Module        | Pi Camera or USB Webcam                |
| Motor Driver         | L298N or similar                       |
| Motors               | DC motors (for movement)               |
| Power Supply         | 5V-12V battery or adapter              |
| Jumper Wires         | For connections                        |
| Breadboard / PCB     | Optional (for stability)               |

---

## 💻 Software Requirements

- **Python 3.7+**
- **OpenCV**
- **RPi.GPIO**
- **NumPy**

All required packages are pre-installed in the custom image.

---

## 📦 Folder Structure


---

## 📥 Raspberry Pi OS Image (with pre-installed software)

Download the custom RPi OS image used in this project from the link below:

🔗 [Download Raspberry Pi Image (Google Drive)](https://drive.google.com/your-image-link)

---

## 🧠 How It Works

1. The Raspberry Pi captures live video from the camera.
2. OpenCV processes the frames and detects specific hand gestures.
3. Detected gestures are mapped to directional commands (e.g., move forward).
4. Based on the command, the Raspberry Pi controls motors via GPIO pins.

---

## 🔌 Wiring Diagram


- Connect GPIO pins to L298N motor driver
- Attach motor driver outputs to chair motors
- Ensure camera module is connected via CSI port or USB

---

## 🚀 Running the Project

### Step 1: Boot from the provided image
- Flash the image to a microSD card
- Insert into Raspberry Pi and boot

### Step 2: Connect hardware as per pin configuration in main.py

### Step 3: Run the code

```bash
cd smart-chair-project
python3 main.py
