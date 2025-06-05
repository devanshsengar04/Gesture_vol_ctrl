# Gesture-Based Volume Control

Control your computer’s volume using hand gestures detected via webcam.

## Features
- Real-time hand tracking using MediaPipe
- Adjust volume by changing distance between fingers
- Visual feedback of volume level

## Author
Devansh Sengar
# ✋ Gesture-Based Volume Control 🎚️

Control your system volume using **hand gestures** in real-time with the help of your webcam!

This project uses **MediaPipe** to detect hand landmarks and **PyCaw** to control the system volume based on the distance between your thumb and index finger.

## 📷 Screenshot Examples

| 0% Volume Gesture        | 40% Volume Gesture         | 100% Volume Gesture            |
|--------------------------|----------------------------|--------------------- ----------|
| ![zero](Images/zero.png) | ![forty](Images/forty.png) | ![hundred](Images/hundred.png) |

---

## 🧠 How It Works

- A webcam feed is captured in real-time.
- MediaPipe detects the hand and tracks landmarks (finger joints).
- The distance between the thumb tip (landmark 4) and index finger tip (landmark 8) is calculated.
- Based on this distance, the system volume is adjusted using PyCaw.
- A green volume bar and volume percentage are shown on the screen for visual feedback.

---

## 🖐️ Hand Landmark Detection

We use Mediapipe's hand tracking solution to identify **21 key landmarks** on each hand. These landmarks help us find where your fingers are and how far apart they are.

![Landmarks](hand_landmarks_docs.png)

---

## 📸 Sample Detected Hand Poses

Real and synthetic hand images with keypoints detected:

![Hand Crops](htm.png)

---

## 🛠️ Technologies Used

| Library       | Purpose                                                 |
|---------------|---------------------------------------------------------|
| **OpenCV**    | For camera access, drawing visuals, and image handling  |
| **MediaPipe** | To detect and track hands using machine learning        |
| **PyCaw**     | To interface with system audio and control volume       |
| **NumPy**     | For numeric computations like interpolation             |
| **math**      | To calculate distances between fingers                  |
| **comtypes**  | To use PyCaw with Windows COM interfaces                |

---

## ▶️ How to Run

### ✅ Requirements
Make sure you have Python installed. Then install the following packages:

```bash
pip install opencv-python mediapipe numpy pycaw comtypes
🧪 Steps
Clone this repository:

bash
Copy
Edit
git clone https://github.com/devanshsengar04/Gesture_vol_ctrl.git
cd Gesture_vol_ctrl
Run the main script:

bash
Copy
Edit
python main.py
Show your hand to the webcam and move your thumb and index finger closer/farther to change the volume.
Press q to quit the program.

🎯 Features
✔️ Real-time gesture detection
✔️ Visual display of landmarks and volume level
✔️ Works directly with system audio (Windows only)
✔️ Fully implemented in Python

❗ Notes
This works only on Windows, as PyCaw uses Windows audio APIs.

Make sure your webcam is working properly.

If the volume bar doesn't show up, ensure your hand is clearly visible to the camera.

📌 Credits
MediaPipe by Google – for hand tracking

PyCaw – for system volume control

OpenCV – for camera and drawing utilities

💡 Future Improvements
Add gesture-based mute/unmute functionality

Support for Linux/macOS using platform-specific audio libraries

Improved UI with animated volume sliders

📬 Contact
Created by: Devansh Sengar
📧 Email: devanshsengar04@gmail.com
🔗 GitHub: @devanshsengar04