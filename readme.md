# 🖐️ Gesture Volume Control using Computer Vision

This project is a **hand gesture-based system volume controller** that lets you increase or decrease the system volume using just your fingers. It uses **OpenCV**, **MediaPipe**, and **PyCaw** libraries to track your hand and control system audio levels in real-time.

---

## 📌 Features

- 👋 Real-time hand detection and finger tracking  
- 🔊 System volume control using finger distance (thumb to index)  
- 🧠 Simple and intuitive user interface  
- 🎯 Accurate detection using MediaPipe’s hand landmarks  
- 💻 Works on Windows  

---

## 🧠 How It Works

1. Captures webcam feed using OpenCV.
2. Detects hand using MediaPipe.
3. Calculates the distance between the **thumb** and **index finger**.
4. Maps the distance to a system volume level using PyCaw.
5. Displays visual feedback on the screen with a volume bar.

---

## 🛠️ Modules Used

![Modules](modules.png)

| Module     | Purpose                                      |
|------------|----------------------------------------------|
| OpenCV     | Webcam capture and image processing          |
| MediaPipe  | Hand landmark detection                      |
| PyCaw      | System audio control                         |
| NumPy      | Mathematical operations                      |
| Comtypes   | Required by PyCaw                            |

---

## ▶️ How to Run

### 📦 Clone the Repository

```bash
git clone https://github.com/devanshsengar04/Gesture_vol_ctrl.git
cd Gesture_vol_ctrl
```

### ✅ Requirements

Make sure Python is installed. Then install the required packages:

```bash
pip install opencv-python mediapipe numpy pycaw comtypes
```

### 🚀 Run the Script

```bash
python main.py
```

---

## 📸 Demo Screenshots

Here are some demo results showing different hand positions and their corresponding volume levels:

| Volume: 0% | Volume: 40% | Volume: 100% |
|------------|-------------|--------------|
| ![0%](zero.png) | ![40%](forty.png) | ![100%](hundred.png) |

---

## 🙋‍♂️ How to Use

1. Open a terminal in the project folder.
2. Run `main.py`.
3. Show your **right hand** to the webcam.
4. Move your **thumb and index finger** closer or farther apart:
   - 🔈 Closer → Lower Volume
   - 🔊 Farther → Higher Volume
5. Press **‘q’** to quit.

---

## 📌 Notes

- Works best in good lighting.
- Background clutter may affect detection accuracy.
- Currently optimized for **right hand only**.

---

## ❤️ Author

**Devansh Sengar**  
🔗 [GitHub](https://github.com/devanshsengar04)

---

<<<<<<< HEAD
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
=======
>>>>>>> a63db5fcc8cc0bda0a44a5e3a987b4c86e2dfe08
