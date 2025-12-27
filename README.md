# Face Detection using OpenCV (Python)

This project demonstrates **real-time face, eye, and smile detection** using **OpenCV** and a webcam. It uses **Haar Cascade Classifiers** to identify facial features from live video frames.

---

## 📌 Project Overview

* Captures live video from the system webcam
* Detects human faces in real time
* Detects eyes and smiles inside detected faces
* Displays bounding boxes and labels on the video feed
* Exits safely on key press

---

## 🛠️ Technologies Used

* Python 3.x
* OpenCV (`cv2`)
* Haar Cascade XML models

---

## 📂 Required Files

Make sure the following files are present in the **same directory** as the notebook/script:

```
haarcascade_frontalface_default.xml
haarcascade_eye.xml
haarcascade_smile.xml
```

These files are required for detecting faces, eyes, and smiles.

---

## ⚙️ How It Works (Step-by-Step)

1. Open the default webcam using OpenCV
2. Read frames continuously
3. Flip the frame horizontally (mirror effect)
4. Convert the frame to grayscale
5. Detect faces using Haar Cascade
6. For each detected face:

   * Detect eyes
   * Detect smiles
7. Draw rectangles and labels on detected features
8. Display the live video feed
9. Press **`q`** to quit the application

---

## 🧠 Detection Parameters Explained

* **scaleFactor = 1.1**
  Reduces image size by 10% at each scale for better detection

* **minNeighbors = 5**
  Higher value reduces false positives

---



## 🚀 How to Run

1. Install OpenCV:

```bash
pip install opencv-python
```

2. Place Haar cascade XML files in the project folder
3. Run the notebook or script
4. Press **`q`** to exit

---

## ✅ Output

* Green rectangle around detected faces
* Text labels:

  * `Eyes Detected`
  * `Smiling`

---

## ⚠️ Common Issues

* **No face detected** → Check XML file paths
* **Webcam not opening** → Change `VideoCapture(0)` to `VideoCapture(1)`
* **Laggy video** → Reduce detection scale or webcam resolution

---

## 📌 Notes

* Haar cascades work best in good lighting
* Smile detection may be less accurate than face detection

---

