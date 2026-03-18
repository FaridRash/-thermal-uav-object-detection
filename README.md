🔥 Thermal UAV Object Detection (HIT-UAV)

📌 Overview

This project focuses on object detection in infrared thermal imagery
captured by UAVs, using the HIT-UAV dataset. The goal is to build a
robust detection model capable of identifying objects under challenging
real-world conditions such as varying altitude, camera angles, and
lighting (day/night).

The dataset includes diverse scenarios such as: - Schools
- Parking lots
- Roads
- Playgrounds

------------------------------------------------------------------------

📊 Dataset

HIT-UAV: A High-Altitude Infrared Thermal Dataset for UAVs

-   2898 thermal images extracted from 43,470 frames
-   Captured from UAV platforms
-   Altitude range: 60–130 meters
-   Camera angle: 30°–90°
-   Conditions: day and night

Classes:

-   Person
-   Bicycle
-   Car
-   OtherVehicle

Source: GitHub:
https://github.com/suojiashun/HIT-UAV-Infrared-Thermal-Dataset
Paper: https://arxiv.org/abs/2204.03245

------------------------------------------------------------------------

🗂️ Data Format

YOLO format:

class_id x_center y_center width height

-   Coordinates normalized to [0, 1]
-   Each image has a corresponding .txt annotation file

------------------------------------------------------------------------

🎯 Objectives

-   Train an object detection model on thermal UAV imagery
-   Evaluate performance across altitude, angle, and lighting conditions
-   Analyze challenges of low-resolution thermal data

------------------------------------------------------------------------

🧠 Methodology

-   Model: YOLO-based detector (e.g., YOLOv8)
-   Pipeline:
    1.  Data preprocessing
    2.  Training
    3.  Validation
    4.  Evaluation (mAP, precision, recall)

------------------------------------------------------------------------

⚙️ Project Structure

data/ images/ labels/ configs/ models/ notebooks/ src/

------------------------------------------------------------------------

📈 Evaluation Metrics

-   Mean Average Precision (mAP)
-   Precision / Recall
-   Class-wise performance

------------------------------------------------------------------------

🚀 Future Work

-   Improve detection of small objects
-   Apply thermal-specific data augmentation
-   Domain adaptation (RGB → Thermal)
-   Edge deployment on UAV systems

------------------------------------------------------------------------

🧩 Why This Project Matters

Thermal UAV detection is important for: - Surveillance and security -
Search and rescue - Traffic monitoring - Autonomous aerial systems

------------------------------------------------------------------------

📜 Citation

Suo et al., HIT-UAV: A High-Altitude Infrared Thermal Dataset for UAVs,
2022.
