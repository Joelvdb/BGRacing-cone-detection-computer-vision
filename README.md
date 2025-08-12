# Cone Detection Model (YOLOv5)

This project is a YOLOv5-based object detection model trained to detect **traffic cones**.

---

## 📊 Results

| Metric            | Value |
| ----------------- | ----- |
| **Precision (P)** | 0.909 |
| **Recall (R)**    | 0.890 |
| **mAP@0.5**       | 0.932 |
| **mAP@0.5:0.95**  | 0.561 |
| **Images used**   | 122   |
| **Instances**     | 202   |

---

## 📂 Dataset

The dataset used for training was collected from [insert dataset source or link here] and contains **only one class: cone**.  
Images were annotated in YOLO format, with bounding boxes around each cone.

---

## 🛠 Training Details

- **Architecture:** YOLOv5s  
- **Image Size:** 640×640  
- **Batch Size:** 8  
- **Epochs:** 50  
- **Optimizer:** SGD (default YOLOv5 settings)  
- **Command Used:**
```
bash
!python /content/yolov5/train.py \
    --workers 8 \
    --img 640 \
    --batch 8 \
    --epochs 50 \
    --data /content/yolov5/data.yaml \
    --weights yolov5s.pt
```

---

## Demo

[![Cone Detection Video](https://github.com/Joelvdb/BGRacing-cone-detection-computer-vision/blob/main/Screenshot%202025-08-12%20at%2013.50.58.png)](https://github.com/Joelvdb/BGRacing-cone-detection-computer-vision/blob/main/cone-detection-video.mp4)

---

