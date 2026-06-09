# Indian Smart Traffic Analytics System

## Project Overview
This project is a computer vision-based traffic analytics system developed using YOLOv8. It detects, classifies, and analyzes vehicles from traffic videos. The system processes video frames and generates insights such as vehicle count and traffic density for real-world smart traffic monitoring applications.

---

## Dataset Description
The project uses Kaggle and Roboflow datasets for training and evaluation.

Source dataset:
/kaggle/input/datasets/dataclusterlabs/indian-vehicle-dataset/Indian_vehicle_dataset

The dataset was annotated using Roboflow to generate bounding box labels for YOLOv8 training.

Annotated dataset:
/kaggle/input/datasets/tanya24jain/indian-vehicle-detection-dataset-for-yolov8/train

For testing and evaluation, unseen real-world traffic videos were used.

/kaggle/input/datasets/tanya24jain/real-world-unseen-traffic-video-dataset/unseen_test_videos

Note: Full datasets are not included in this repository due to size limitations. Only sample data and outputs are provided.

---

## Model Training (YOLOv8)
The YOLOv8 model was trained on a custom annotated dataset for multi-class vehicle detection.

Training process:
- Pre-trained YOLOv8 model (transfer learning) was used
- Custom dataset in YOLO format with bounding box annotations
- Model trained for multiple vehicle classes (Car, Bike, Bus, Truck, Autorickshaw)
- Training performed in Kaggle GPU environment
- Hyperparameters tuned for better performance

Output of training:
- Best trained weights saved as best.pt
- Model learned accurate detection of multiple vehicle types

---

## Features
- Real-time vehicle detection
- Vehicle classification
- Vehicle counting
- Traffic density analysis
- Video-based inference
- Evaluation on unseen data

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
1. Dataset collection from Kaggle
2. Frame extraction from traffic videos
3. Dataset annotation using Roboflow
4. YOLOv8 model training
5. Testing on unseen traffic videos
6. Traffic analytics generation

---

## Project Structure
01_Frame_Extraction.ipynb
02_YOLOv8_Training.ipynb
03_Testing_Analytics.ipynb
models/
outputs/
screenshots/

---

## Outputs
- Vehicle detection results
- Traffic density graphs
- Vehicle count analysis
- Final demo video showing inference
- CSV analytics report

---

## Demo
Final output video demonstrates real-time vehicle detection, classification, and traffic analytics on unseen traffic videos.

Add final_demo.mp4

---

## Author
Tanya Jain
M.Tech Computer Science (AI/ML)

---

## Note
This project represents a complete end-to-end computer vision pipeline including dataset preparation, annotation, model training, and testing on real-world unseen data.
