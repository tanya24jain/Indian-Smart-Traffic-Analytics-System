# Indian Smart Traffic Analytics System

## Project Overview
This project is a computer vision-based traffic analytics system that uses YOLOv8 to detect, classify, and analyze vehicles from traffic videos. The system processes video frames, detects multiple vehicle types, and generates insights such as vehicle count and traffic density. It is designed for real-world smart traffic monitoring applications.

---

## Dataset Description
The project uses a Kaggle-based Indian vehicle dataset for training and evaluation.

Source dataset:
`/kaggle/input/datasets/dataclusterlabs/indian-vehicle-dataset/Indian_vehicle_dataset`

The dataset was annotated using Roboflow to create bounding box labels for YOLOv8 training.

Annotated dataset:
`/kaggle/input/datasets/tanya24jain/indian-vehicle-detection-dataset-for-yolov8/train`

For testing and evaluation, unseen real-world traffic videos were used.

Unseen test dataset:
`/kaggle/input/datasets/tanya24jain/real-world-unseen-traffic-video-dataset/unseen_test_videos`

---

## Model Training (YOLOv8)

The YOLOv8 model was trained on the custom annotated dataset for multi-class vehicle detection.

Training process:
- Pre-trained YOLOv8 model (transfer learning) was used
- Custom dataset was provided in YOLO format
- Model was trained using bounding box annotations
- Hyperparameters were tuned for better accuracy
- Training was performed in Kaggle environment using GPU

Output of training:
- Best trained weights saved as `best.pt`
- Model learned to detect multiple vehicle classes accurately

---

## Features
Real-time vehicle detection  
Vehicle classification (Car, Bike, Bus, Truck, Autorickshaw)  
Vehicle counting  
Traffic density analysis  
Video-based inference  
Unseen data evaluation  

---

## Tech Stack
Python  
YOLOv8 (Ultralytics)  
OpenCV  
Pandas  
Matplotlib  
Kaggle / VS Code  

---

## Project Workflow
Dataset collection from Kaggle  
Frame extraction from videos  
Dataset annotation using Roboflow  
YOLOv8 model training  
Testing on unseen traffic videos  
Traffic analytics generation  

---

## Project Structure
01_Frame_Extraction.ipynb  
02_YOLOv8_Training.ipynb  
03_Testing_Analytics.ipynb  

---

## Outputs
Vehicle detection results  
Traffic density graphs  
Vehicle count analysis  
Final demo video  
CSV analytics report  

---

## Demo
Add final_demo.mp4  

---

## Author
Tanya Jain  
M.Tech CSE (AI/ML)
