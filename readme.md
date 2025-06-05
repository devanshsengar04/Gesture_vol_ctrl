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

