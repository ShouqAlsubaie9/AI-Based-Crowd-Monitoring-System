# AI-Based Crowd Monitoring and Anomaly Detection for Large-Scale Events

> Master's Graduation Project

An AI-powered crowd monitoring system designed to improve public safety during large-scale events by combining computer vision, deep learning, and intelligent behavior analysis.

The system performs real-time people detection, multi-object tracking, gender classification, crowd density estimation, and behavioral anomaly detection using state-of-the-art deep learning models.

---

# Project Overview

Managing large crowds at stadiums, concerts, festivals, airports, and public events presents significant safety challenges. Traditional surveillance systems rely heavily on human operators, making it difficult to detect abnormal situations in real time.

This project introduces an intelligent surveillance system capable of automatically monitoring crowd movement and detecting abnormal behaviors to support security personnel in making faster and more informed decisions.

---

# Key Features

✔ Real-time person detection

✔ Multi-object tracking

✔ Gender classification

✔ Crowd counting

✔ Crowd density estimation

✔ Occupancy monitoring

✔ Loitering detection

✔ Abnormal speed detection

✔ Crowd surge detection

✔ Zone-based analytics

✔ Real-time alerts

✔ Live dashboard

✔ Automatic report generation

---

# System Workflow

Video Input

↓

YOLOv8 Detection

↓

ByteTrack Tracking

↓

Vision Transformer Gender Classification

↓

People Counting

↓

Crowd Density Estimation

↓

Behavior Analysis

↓

Real-Time Alerts

↓

Output Dashboard & Reports

---

# Technologies Used

- Python
- YOLOv8
- ByteTrack
- Vision Transformer (ViT)
- OpenCV
- PyTorch
- Hugging Face Transformers
- NumPy
- Pillow (PIL)

---

# Dataset

The system was evaluated using two surveillance datasets.

## Indoor Mall Dataset

- Used for testing
- Approximately 8,000–10,000 extracted video frames
- Medium crowd density

## Custom Outdoor Dataset

- Used for training and testing
- Approximately 12,000–15,000 extracted video frames
- Medium to High crowd density

Overall evaluation was performed using more than **20,000 extracted video frames**. :contentReference[oaicite:0]{index=0}

---

# Detection Performance

| Metric | Result |
|---------|--------|
| Precision | 90% |
| Recall | 88% |
| mAP | 89% |
| Low-Light mAP | 83% |

The detection model demonstrated strong performance in real-world surveillance environments while maintaining reliable real-time processing. :contentReference[oaicite:1]{index=1}

---

# Tracking Performance

- 91% tracking continuity during partial occlusion
- 85% re-identification accuracy
- Low ID switch rate in crowded scenes
- Robust tracking using ByteTrack

:contentReference[oaicite:2]{index=2}

---

# Gender Classification

The Vision Transformer (ViT) model achieved:

**98.7% classification accuracy**

allowing accurate demographic analysis of monitored areas. :contentReference[oaicite:3]{index=3}

---

# Behavior Analysis

The system automatically detects:

- Loitering
- Abnormal Speed
- Crowd Surge

Performance:

| Task | Accuracy |
|------|----------|
| Loitering Detection | 87% |
| Abnormal Speed Detection | 90% |
| Crowd Surge Detection | 92% |

:contentReference[oaicite:4]{index=4}

---

# Output

The system provides:

- Annotated surveillance videos
- Live dashboard
- Crowd statistics
- Gender statistics
- Occupancy information
- Crowd alerts
- Summary reports

---

# Folder Structure

```text
AI-Based-Crowd-Monitoring-System
│
├── src/
├── models/
├── datasets/
├── screenshots/
├── results/
├── demo/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Future Improvements

- Face Recognition
- Thermal Camera Support
- Multi-Camera Tracking
- Weapon Detection
- Cloud Deployment
- Mobile Dashboard
- Real-Time Notifications

---

# Screenshots

> Add screenshots demonstrating:

- Person Detection
- Tracking IDs
- Gender Classification
- Crowd Density Dashboard
- Loitering Detection
- Crowd Surge Alerts
- Heatmaps

---

# Author

**Shouq Alsubaie**

Master's Degree in Cybercrime and Digital Forensic Investigation

Interested in:

- Security Operations (SOC)
- Digital Forensics
- Computer Vision
- Artificial Intelligence
- Threat Intelligence
