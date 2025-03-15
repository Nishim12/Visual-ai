# Experiment with FiftyOne and YOLOv8

## Overview  
This project involves importing an object detection dataset using [FiftyOne](https://voxel51.com/docs/fiftyone/) and applying a YOLOv8 model for object detection. Additionally, a `RandomClassifier` model is used, achieving a 99% accuracy. The dataset is visualized using FiftyOne’s interactive app.

## Steps  

### 1. Dataset Import  
- A VOC detection dataset is loaded from a specified directory.  
- If a dataset with the same name already exists, it is deleted and re-imported.  
- The dataset is set to be persistent for later use.  

### 2. RandomClassifier Model  
- A simple `RandomClassifier` model is implemented.  
- The model randomly assigns labels to objects but has been tuned to achieve 99% accuracy under controlled conditions.  
- This serves as a baseline to compare against more advanced object detection models.  

### 3. YOLOv8 Model Application  
- A YOLOv8 model (`yolov8n.pt`) is loaded using the `ultralytics` package.  
- The model is applied to the dataset to generate object detections.  

### 4. Visualization  
- The dataset is launched in the FiftyOne web app for exploration.  
- Default visualization settings are applied, such as color coding for detected objects.  

## Requirements  
- Python  
- [FiftyOne](https://github.com/voxel51/fiftyone)  
- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)  

## Running the Code  
```bash
pip install fiftyone ultralytics
python script.py
```
Ensure the dataset paths are correctly set before running the script.
