# Hand Finger Counter Using MediaPipe & OpenCV

This project is a real-time hand finger counting system using **MediaPipe Hands** and **OpenCV**.  
It detects one or two hands from a webcam feed and calculates the total number of raised fingers.

## 🚀 Features
- Real-time hand detection using webcam
- Supports up to **two hands**
- Accurate finger counting using landmark positions
- Left and right hand differentiation
- Mirrored camera view for natural interaction

## 🧠 How It Works
MediaPipe provides **21 hand landmarks** for each detected hand.  
Finger counting is performed by comparing the fingertip position with its corresponding joint:
- **Thumb**: Uses horizontal (x-axis) comparison and adapts to left/right hand
- **Other fingers**: Uses vertical (y-axis) comparison between fingertip and PIP joint

The total number of raised fingers from all detected hands is displayed on the screen in real time.

## 🛠️ Technologies Used
- Python
- OpenCV
- MediaPipe

## 📦 Requirements
Make sure you have Python installed, then install the required libraries:

```bash
pip install opencv-python mediapipe
