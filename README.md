# 🚁 Drone Traffic Object Detection & Tracking

Real-time drone traffic object detection and tracking using YOLOv8, ByteTrack, OpenCV and VisDrone dataset.

---

## 📌 Features

- Real-time object detection
- Multi-object tracking
- Drone traffic analysis
- Vehicle and pedestrian detection
- Video inference pipeline

---

## 🧠 Technologies Used

- Python
- YOLOv8
- OpenCV
- ByteTrack
- PyTorch
- Google Colab

---

## 📂 Dataset

VisDrone Dataset:

https://github.com/VisDrone/VisDrone-Dataset

---

## 🚀 Installation

```bash
pip install ultralytics opencv-python torch torchvision numpy
```

---

## ▶️ Run Detection

```python
from ultralytics import YOLO

model = YOLO("best.pt")

results = model.predict(
    source="test_video.mp4",
    conf=0.7,
    imgsz=640,
    save=True
)
```

---

## ▶️ Run Tracking

```python
from ultralytics import YOLO

model = YOLO("best.pt")

results = model.track(
    source="test_video.mp4",
    tracker="bytetrack.yaml",
    conf=0.7,
    imgsz=640,
    save=True
)
```

---

## 📊 Model Performance

- YOLOv8 + ByteTrack
- Trained/Fine-tuned on VisDrone Dataset
- Optimized for drone traffic scenes

---

## 👨‍💻 Author

**Gaurav Sharma**

LinkedIn:
www.linkedin.com/in/gauravnitrkl

GitHub:
https://github.com/jontyroades2006-lang
