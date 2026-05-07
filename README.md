# AI-Based Plastic Waste Detection using YOLOv8

## Project Overview
This project presents an AI-based object detection system developed using YOLOv8 to identify and classify waste materials such as plastic, bio, and rov from images. The system is designed to support automated waste detection using deep learning techniques.

## Objective
The main objective of this project is to build a computer vision model capable of detecting and localising different types of waste objects within images, and to evaluate its performance using standard metrics.

## Dataset
The Trash-ICRA19 dataset was used for training and evaluation. It contains labelled images with bounding boxes for three classes:
- Plastic
- Bio
- Rov

The dataset is organised into training, validation, and testing sets in YOLO format.

## Model
The YOLOv8 architecture from the Ultralytics framework was used for object detection. The baseline model uses the YOLOv8n variant, which is lightweight and efficient.

## Experiments
The project includes multiple experiments conducted by different team members:
- Baseline model (YOLOv8n)
- Image size variation
- Model comparison (YOLOv8n vs YOLOv8s)
- Data augmentation
- Final optimised model

## Evaluation Metrics
The model performance was evaluated using:
- Precision
- Recall
- mAP50
- mAP50-95

## Challenges
Some challenges faced during the project include:
- Large dataset handling and training time
- Dataset organisation into correct YOLO format
- Performance imbalance across classes, particularly for the bio class

## Conclusion
The baseline model performed well for plastic detection but showed limitations in detecting bio and rov classes. Further improvements were explored through experimentation with model configurations and training strategies.

## Tools and Technologies
- Python
- Google Colab
- Ultralytics YOLOv8
- GitHub

## Contributors
- Dulmi Tharundya Narasinghe - 12267791
- Liam Scott - 12290871
- Manan Bharatbhai Patel - 12278672
- Md Nur Alam Islam Nafi - 12298910
  
-Tanjim Ahmed Mahi - 12298057
