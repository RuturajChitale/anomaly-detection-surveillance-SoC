# Anomaly Detection in Surveillance Videos

## Overview

This project presents an end-to-end pipeline for detecting anomalous activities in surveillance videos using deep learning and computer vision techniques. The system combines object detection, multi-object tracking, trajectory feature extraction, and unsupervised anomaly detection to identify unusual movements in video sequences.

---

## Project Workflow

The complete pipeline consists of the following steps:

1. Train a YOLOv5 model for object detection.
2. Detect objects in surveillance videos.
3. Track detected objects across frames using ByteTrack.
4. Extract trajectory-based features such as displacement, velocity, and acceleration.
5. Apply Isolation Forest on the extracted features to identify abnormal trajectories.
6. Evaluate the model using Precision, Recall, F1-Score, and Confusion Matrix.
7. Visualize the detected anomalies and tracked objects.

---

## Technologies Used

* Python
* YOLOv5
* ByteTrack
* OpenCV
* PyTorch
* Scikit-learn
* NumPy
* Pandas
* Matplotlib

---

## Project Files

* **model_training.ipynb** – Training the YOLOv5 object detection model.
* **inference_and_tracking.ipynb** – Object detection, tracking, feature extraction, anomaly detection, and evaluation.

---

## Results

The project successfully performs:

* Object detection on surveillance videos.
* Multi-object tracking using ByteTrack.
* Trajectory feature extraction.
* Unsupervised anomaly detection using Isolation Forest.
* Performance evaluation using standard classification metrics.
* Visualization of tracked objects and detected anomalies.

---

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open `model_training.ipynb` to train the detection model (or use the provided trained weights).
4. Open `inference_and_tracking.ipynb` to perform detection, tracking, anomaly detection, and evaluation on surveillance videos.

---

## Acknowledgements

This project uses YOLOv5 for object detection, ByteTrack for multi-object tracking, and Isolation Forest for anomaly detection. The implementation is developed for educational and research purposes.

