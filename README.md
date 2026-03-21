Gesture Volume Control

Description

This project controls system volume using hand gestures through a webcam.
It uses MediaPipe hand landmarks to detect the distance between thumb and
index finger and updates volume in real time.

Technologies Used

- Python
- OpenCV
- MediaPipe
- Flask
- pyautogui (sends volume up/down key presses)
- pycaw (reads current system volume for UI display)

How it Works

- Webcam captures live video frames.
- MediaPipe detects hand landmarks.
- Distance between thumb tip and index tip is calculated.
- Small distance triggers volume down.
- Large distance triggers volume up.
- Mid range keeps volume hold.

Prerequisites

- Python 3.9+
- Webcam
- Windows OS (recommended/tested)

Run Project

1. Install dependencies:
   pip install -r requirements.txt

2. Run the application:
   python app.py

3. Open browser:
   http://127.0.0.1:5000

API Endpoints

- GET / -> Main page
- GET /start -> Start webcam capture
- GET /stop -> Stop webcam capture
- GET /video -> Live MJPEG stream
- GET /volume -> Current system volume percentage
- GET /gesture -> Current gesture and detection status

Features

- Real-time gesture-based volume control
- Live webcam preview in browser
- Horizontal and vertical volume indicators
- Start and stop camera controls

Team Members

- Alok Kumar Agrahari
- Gokul
- Gouri
- Shubh Sahu
- Sabarinath KR