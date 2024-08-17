## Project Description
The **Motorcycle Classification** project aims to detect and classify motorcycles in images into five categories: **Honda**, **Suzuki**, **Yamaha**, **VinFast**, and **Others**. The project uses the **YOLOv8n** model by Ultralytics for motorcycle detection and classification.
This is my Final Project in Mechina Learning(CS114) at university 

## Process Overview
The project consists of the following steps:

1. **Motorcycle Detection in Images:**
   - The YOLOv8n model is used to detect motorcycles in images.
   - The detection process outputs the bounding boxes containing the motorcycles, along with their positions and dimensions.

2. **Create COCO-formatted Data Files:**
   - The detection results are stored in **COCO format**, with the following fields:
     - `label`: The motorcycle category (0: Others, 1: Honda, 2: Suzuki, 3: Yamaha, 4: VinFast).
     - `center_x`: The x-coordinate of the bounding box center.
     - `center_y`: The y-coordinate of the bounding box center.
     - `bbox_width`: The width of the bounding box.
     - `bbox_height`: The height of the bounding box.

3. **Train the Model:**
   - The YOLOv8n model is trained on the prepared dataset in COCO format.
   - The training process includes data preprocessing, model training, and hyperparameter tuning.

4. **Evaluate the Model:**
   - After training, the model is evaluated on a validation dataset to measure accuracy, recall, and other performance metrics.
   - The evaluation results are used to improve the model.

## Installation Requirements
- **Python 3.x**
- **Ultralytics YOLOv8**
