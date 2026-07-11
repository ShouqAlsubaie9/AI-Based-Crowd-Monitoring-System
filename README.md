# AI-Based Crowd Monitoring and Anomaly Detection for Large-Scale Events

> Master's Graduation Project

An intelligent AI-powered surveillance system developed to monitor crowded environments and support security personnel through real-time crowd analysis, behavior monitoring, and anomaly detection.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-red)
![ByteTrack](https://img.shields.io/badge/ByteTrack-Multi--Object%20Tracking-green)
![Vision Transformer](https://img.shields.io/badge/Vision%20Transformer-ViT-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-lightgrey)

---

# Project Overview

Large public events such as concerts, sports matches, festivals, and exhibitions require continuous monitoring to ensure crowd safety. Manual surveillance is often inefficient due to the large number of people and the difficulty of identifying abnormal situations in real time.

This project presents an AI-based crowd monitoring system that combines computer vision and deep learning techniques to automate crowd analysis. The system performs real-time head detection, multi-object tracking, gender classification, crowd density estimation, occupancy monitoring, and behavioral anomaly detection to improve situational awareness and support security decision-making.

Unlike conventional surveillance systems that rely on full-body detection, this project utilizes a custom-trained YOLOv8 head detection model. Head detection provides more reliable performance in crowded environments where people are frequently affected by body occlusion, allowing the system to maintain accurate counting and tracking.

---

# Key Features

- Real-time head detection using a custom-trained YOLOv8 model
- Multi-object tracking with ByteTrack
- Gender classification using Vision Transformer (ViT)
- Crowd counting
- Crowd density estimation
- Occupancy monitoring
- Zone-based crowd analytics
- Loitering detection
- Abnormal speed detection
- Crowd surge detection
- Live visual monitoring dashboard
- Automatic statistical reporting

---

# Why Head Detection?

Traditional person detection models often experience reduced accuracy in crowded environments because people partially block each other.

To overcome this limitation, the proposed system detects heads instead of full bodies. Since heads remain visible in highly crowded scenes, this approach significantly improves detection robustness, tracking continuity, and crowd counting accuracy in high-density environments such as stadium entrances and event gates.

---

# System Workflow

```
Video Input
      │
      ▼
YOLOv8 Head Detection
      │
      ▼
ByteTrack Multi-Object Tracking
      │
      ▼
Vision Transformer Gender Classification
      │
      ▼
Crowd Counting & Density Estimation
      │
      ▼
Behavior Analysis
(Loitering • Speed • Crowd Surge)
      │
      ▼
Real-Time Dashboard & Reports
```

---

# Technologies Used

## Programming

- Python
- OpenCV
- NumPy
- Pillow (PIL)

## Deep Learning

- YOLOv8
- ByteTrack
- Vision Transformer (ViT)
- PyTorch
- Hugging Face Transformers

---

# Core Modules

## Head Detection

A custom-trained YOLOv8 model detects human heads in surveillance footage to improve detection performance under crowded conditions.

---

## Multi-Object Tracking

ByteTrack assigns a unique ID to each detected individual and maintains identity consistency across video frames.

---

## Gender Classification

Detected head regions are classified using a Vision Transformer (ViT) model to estimate gender distribution within monitored areas.

---

## Crowd Analytics

The system continuously analyzes crowd movement and provides:

- Total crowd count
- Zone occupancy
- Crowd density estimation
- Area statistics

---

## Behavioral Analysis

The monitoring framework identifies abnormal crowd behaviors including:

- Loitering
- Abnormal walking speed
- Crowd surge

These events are highlighted in real time to assist security personnel.

---

# Dataset

The system was evaluated using two surveillance datasets.

### Indoor Mall Dataset

- Used for testing
- Approximately 8,000–10,000 extracted video frames
- Medium crowd density

### Custom Outdoor Dataset

- Used for training and testing
- Approximately 12,000–15,000 extracted video frames
- Medium to high crowd density

Overall evaluation was conducted using more than **20,000 extracted video frames**.

---

# Project Structure

```
AI-Based-Crowd-Monitoring-System
│
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
│
├── src/
│
├── models/
│
├── datasets/
│
├── screenshots/
│
├── results/
│
├── demo/
│
└── docs/
```

---

# Results

The proposed system successfully demonstrated the ability to:

- Detect individuals in crowded environments using head detection
- Maintain consistent tracking with ByteTrack
- Classify gender using Vision Transformer
- Estimate crowd density in real time
- Detect loitering behavior
- Detect abnormal movement speed
- Detect crowd surge events
- Generate visual analytics for crowd monitoring

---

# Future Improvements

Future development may include:

- Face recognition integration
- Multi-camera tracking
- Weapon detection
- Cloud deployment
- Mobile monitoring dashboard
- Real-time notification system
- Thermal camera support

---

# Screenshots

Add screenshots demonstrating:

- Head Detection
- Multi-Object Tracking
- Gender Classification
- Crowd Density Estimation
- Loitering Detection
- Crowd Surge Detection
- Dashboard Interface

---

# Disclaimer

This repository represents the implementation of my Master's graduation project. Certain datasets, trained models, or supporting files may not be included due to academic or licensing restrictions.

---

# Author

**Shouq Alsubaie**

Master's in Cybercrime and Digital Forensic Investigation

**Areas of Interest**

- Cybersecurity
- Security Operations (SOC)
- Digital Forensics
- Threat Intelligence
- Artificial Intelligence
- Computer Vision
