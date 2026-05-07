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

## Installation and Execution

### Requirements
The project was developed using Python and Google Colab with GPU acceleration.

Required libraries include:
- ultralytics
- torch
- torchvision
- opencv-python
- matplotlib
- pandas
- numpy

### Running the Project
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Enable GPU runtime in Google Colab:
   Runtime → Change Runtime Type → GPU
3. Install required libraries if necessary:
```python
pip install ultralytics

4. Mount Google Drive if running in Colab
from google.colab import drive
drive.mount('/content/drive')

5. Update dataset paths if required.
6. Run notebook cells sequentially from top to bottom.

###Outputs
The notebook generates:

-trained model weights
-prediction images
-confusion matrices
-evaluation metrics
-training graphs

## Final Optimised Configuration
The final selected configuration included:
- YOLOv8n
- Image size: 512
- Epochs: 30
- Batch size: 8
- Data augmentation enabled

This configuration achieved the best balance between:
- Precision
- Recall
- mAP performance
- Computational efficiency
- Training time

## Challenges and Lessons Learned
-Several technical and computational challenges were encountered during the project.
-Initially, some experiments were accidentally executed using CPU instead of GPU acceleration, resulting in extremely long training durations. Through experimentation, the importance of GPU-based deep learning training and computational efficiency became clear.
-Google Colab runtime resets and GPU usage limitations occasionally interrupted training sessions, requiring experiments to be rerun multiple times. This highlighted the importance of saving outputs, model weights, and experiment results directly to Google Drive.
-Additional challenges included debugging coding errors, resolving dataset path issues, and managing shared datasets and experiment outputs across multiple group members and branches.

These challenges improved understanding of:
- GPU acceleration,
- cloud-based machine learning environments,
- experiment management,
- debugging,
- and collaborative AI development workflows.

## Repository Structure
Each group member conducted specific controlled experiments within separate GitHub branches.
The main branch contains:
- final notebooks
- presentation materials
- documentation
Experimental and development work remains available within individual member branches.

## Conclusion
The baseline model performed well for plastic detection but showed limitations in detecting bio and rov classes. FControlled experiments involving image size, training duration, augmentation, and model variants were conducted to analyse performance differences and computational trade-offs. The final optimised YOLOv8n configuration achieved improved detection performance while maintaining computational efficiency and practical deployment suitability. The project demonstrated the importance of balancing detection accuracy with GPU usage, training time, and overall computational cost during model optimisation.

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
