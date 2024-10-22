# Alejandro Paredes La Torre, Object Detection Project

## Overview
This project focuses on implementing and evaluating two prominent object detection models: **Faster R-CNN** and **YOLOv8**. Both models are trained on a custom dataset containing various objects, including laptops, keyboards, mice, and utensils. The objective is to assess their performance in terms of accuracy, speed, and overall effectiveness in real-world scenarios.

## Models Implemented

### Faster R-CNN
- **Architecture**: Combines region proposal networks with end-to-end training for effective object detection.
- **Performance**:
  - Mean IoU: **0.8350**
  - F1 Score: **0.8716** on the testing set
- **Key Techniques**:
  - Emphasis on precise annotation and data augmentation.
  - Utilized a dataset annotated using Roboflow.

### YOLOv8
- **Architecture**: Employs a unified approach for real-time object detection by predicting bounding boxes and class probabilities in one pass.
- **Performance**:
  - Mean Average Precision (mAP) at IoU=0.50: **0.947**
  - mAP at IoU=0.50:0.95: **0.758**
- **Key Techniques**:
  - Advanced augmentations applied during training for improved adaptability.
  - Demonstrated remarkable speed and efficiency, making it suitable for real-time applications.

## Dataset
- The dataset includes images of laptops, keyboards, mice, and utensils.
- Each object is annotated with bounding boxes to provide accurate training data.
- The dataset is split into:
  - **Training Set**: 80% (1732 images)
  - **Validation Set**: 20% (433 images)

## Results Summary
- **Faster R-CNN**:
  - Effective in generating reliable predictions with a focus on precise annotation.
  
- **YOLOv8**:
  - Excels in speed and efficiency, suitable for real-time detection scenarios, adapting well to the dataset with advanced augmentations.

## Conclusion
Both Faster R-CNN and YOLOv8 showcase significant strengths in object detection tasks. Their performances highlight the critical role of dataset quality and annotation in training robust models, ultimately contributing to advancements in computer vision applications.

## Requirements
- Python 3.x
- PyTorch
- torchvision
- Roboflow for dataset management

## Installation
```bash
pip install torch torchvision roboflow
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.