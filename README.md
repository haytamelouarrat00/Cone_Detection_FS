# **Custom Cone Detection Model for Formula Student Perception Module**

This repository contains a custom-trained object detection model built for detecting custom Formula Student Cones in a High Speed situationship. The model was trained using YOLOv11s, with performance and training visualizations included.

---

## **Table of Contents**
1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Training Process](#training-process)
4. [Validation Results](#validation-results)
5. [Performance Metrics](#performance-metrics)
6. [Results](#results)

---

## **Overview**
This repository demonstrates the training and evaluation of a custom object detection model. Below are some highlights:
- **Framework Used**: YOLOv11s
- **Dataset**: https://universe.roboflow.com/fsbdriverless-xi0fv/fsai-11-03-2024
- **Performance Metrics**: Precision, recall, and F1-score analyzed in-depth.
- **Visualizations**: Training/validation batches, confusion matrices, and metric curves are included.

---

## **Dataset**
### **Class Distribution**
Below is the label distribution of the dataset:

![Labels Overview](./res/labels.jpg)

### **Correlogram**
The relationship between classes in the dataset is visualized here:

![Labels Correlogram](./res/labels_correlogram.jpg)

---

## **Training Process**
### **Training Batches**
Sample images from the training data:

![Training Batch 0](./res/train_batch0.jpg)
![Training Batch 1](./res/train_batch1.jpg)

### **Training Results**
Training and validation loss over epochs:

![Training Results](./res/results.png)

---

## **Validation Results**
### **Validation Samples**
Below are samples from the validation set with ground truth and predicted labels:

**Ground Truth:**  
![Validation Batch 0 - Labels](./res/val_batch0_labels.jpg)

**Predictions:**  
![Validation Batch 0 - Predictions](./res/val_batch0_pred.jpg)

---

## **Performance Metrics**
### **Confusion Matrix**
The confusion matrix shows how well the model distinguishes between classes:

![Confusion Matrix](./res/confusion_matrix.png)

### **Normalized Confusion Matrix**
Normalized confusion matrix for a clearer class-by-class accuracy breakdown:

![Normalized Confusion Matrix](./res/confusion_matrix_normalized.png)

### **Precision-Recall Curves**
**Precision-Recall (PR) Curve:**
![PR Curve](./res/PR_curve.png)

**Precision (P) Curve:**
![P Curve](./res/P_curve.png)

**Recall (R) Curve:**
![R Curve](./res/R_curve.png)

**F1-Score Curve:**
![F1 Curve](./res/F1_curve.png)

## **Results**
The model achieved an F1-score of 0.92 on the validation set. The model is now ready for deployment and testing in real-world scenarios.
The input this model was tested on was a video feed from a [Youtube video of **Chalmers Formula Student**](https://www.youtube.com/watch?v=sQ7gVgm-L28).

[MP4 Results Video](./results.mp4)

