# Construction-Site-Safety-Detection-System-based-on-YOLOv8-and-Transfer-Learning.
<img width="1402" height="1122" alt="construction" src="https://github.com/user-attachments/assets/3a6026a9-6c21-47c0-9174-070d974fa0fa" />

## Overview

This project is a Computer Vision and Deep Learning based safety monitoring system that detects Personal Protective Equipment (PPE) compliance on construction sites using YOLOv8.

The model identifies workers, safety equipment, and safety violations from images and videos in real time.

---

## Features

* Detect Hard Hats
* Detect Safety Vests
* Detect Face Masks
* Detect Workers
* Detect Vehicles
* Detect Machinery
* Identify PPE Violations
* Real-Time Image Detection
* Video-Based Safety Monitoring

---

## Dataset

Dataset Source:

https://www.kaggle.com/datasets/snehilsanyal/construction-site-safety-image-dataset-roboflow

Classes:

* Hardhat
* Mask
* NO-Hardhat
* NO-Mask
* NO-Safety Vest
* Person
* Safety Cone
* Safety Vest
* Machinery
* Vehicle

---

## Technologies Used

* Python
* YOLOv8
* Ultralytics
* OpenCV
* NumPy
* Matplotlib
* KaggleHub
* Google Colab

---

## Deep Learning Model

Model Used:

YOLOv8 Nano (yolov8n.pt)

Task:

Object Detection

Learning Technique:

Transfer Learning

---

## Training Configuration

* Epochs: 50
* Image Size: 640 × 640
* Batch Size: 16
* Optimizer: Auto
* Early Stopping Patience: 15

---

## Installation

```bash
pip install ultralytics
pip install kagglehub
pip install pyyaml
pip install opencv-python
pip install matplotlib
pip install numpy
```

## Run Training

```python
from ultralytics import YOLO

model = YOLO("yolov8n.pt")

model.train(
    data="ppe_data.yaml",
    epochs=50,
    imgsz=640
)
```

## Project Outcome

The trained model can automatically detect PPE compliance and safety violations in construction environments, helping improve workplace safety and monitoring.

## Author

FANI 2323
Computer Science Undergraduate
Machine Learning & Computer Vision Enthusiast
