# 🎨 Real-Time Color Recognition using OpenCV

A Python project using **OpenCV** to detect and track specific color objects (Blue) in real-time using a webcam stream.

---

## 📌 Task Overview
This repository contains the implementation of the **Color Recognition** task assigned by SmartMethods using OpenCV.

---

## 🛠️ Features & Methodology
1. **Live Video Capture:** Continuously captures frames from the webcam.
2. **Color Space Transformation:** Converts video frames from BGR to **HSV** (Hue, Saturation, Value) color space for precise color segmentation.
3. **Color Thresholding:** Applies a binary mask to detect target colors within defined HSV bounds:
   - **Lower Limit:** `[90, 50, 50]`
   - **Upper Limit:** `[130, 255, 255]`
4. **Contour Analysis & Noise Filtering:** Tracks target boundaries while filtering out background noise using an area threshold of `area > 500`.
5. **Real-Time Bounding Box:** Overlays a rectangular frame and label (`Blue Color Detected`) on the detected object.

---

## 🚀 How to Run

### Prerequisites
Make sure Python 3 and the required libraries are installed:

pip install opencv-python numpy

### Execution
Run the main script:

python main.py

> **Note:** Grant camera permissions when prompted. Press **`q`** on the display window to exit.
