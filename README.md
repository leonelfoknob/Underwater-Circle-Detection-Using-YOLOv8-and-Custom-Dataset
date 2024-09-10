# Underwater-Circle-Detection-Using-YOLOv8-and-Custom-Dataset

This project focuses on detecting circles underwater using a custom-trained YOLOv8 model. Data was collected using a GoPro camera mounted on an underwater robot, and the model was trained to achieve high accuracy for real-world underwater applications.

Project Video:
- [Include link to project video if available on YouTube or other platforms]

Components and Tools:
- Underwater Robot:
Purpose: The robot, equipped with a GoPro camera, was used to capture video footage underwater. This footage was essential for creating the custom dataset.
Photo: [Include a photo of the underwater robot here]
- GoPro Camera:
Data Collection: Used to capture high-quality underwater footage for the dataset, providing clear visuals for accurate labeling and training.
- Roboflow:
Data Labeling: Roboflow was used to label the collected footage, identifying circles in the underwater environment. This step was crucial for preparing the data to train the YOLOv8 model.
- YOLOv8 (yolovon.pt):
Model Training: A custom YOLOv8 model was trained using the labeled dataset. The model was optimized to detect circles with high accuracy in underwater settings.
Accuracy: The trained model achieved a remarkable accuracy of 98%, making it highly effective for underwater detection tasks.

Files and Configuration:
- config.yaml:
This file contains the parameters used during training, including class names and the paths for both training and validation data. These configurations are essential for setting up the training environment.
- custom_dataset_yolo_train.py:
This Python script is responsible for training the custom YOLOv8 model. It processes the dataset, configures the model parameters, and performs the training process.
- custom_data_predict.py:
This script is used to make predictions using the trained model. For demonstration purposes, a video file is used, but the model is also capable of performing real-time predictions using a live camera feed.

Training and Model Files:

After the training process, the resulting custom model can be found in the directory: runs\detect\yolov8n_custom\weights. This folder contains two important files:
- best.pt: The best-performing model during training.
- last.pt: The most recent version of the model after training.

Real-World Applications:

This model can be adapted for real-time use with underwater robots to detect circles or similar objects. The combination of the robot and the YOLOv8 model makes it versatile for tasks such as underwater inspections or object recognition.
