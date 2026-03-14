# 🧠 Brain Tumor MRI Classification & Explainable AI

## Overview

This project implements a deep learning pipeline for **brain tumor detection and classification** from MRI scans, featuring:

- **CNN Architectures:** VGG16, ResNet50, EfficientNetB0
- **Dataset:** 7,023 MRI images, 4 tumor categories (glioma, meningioma, pituitary, no-tumor)
- **Training:** Transfer learning, data augmentation, class balancing, staged fine-tuning
- **Metrics:** Accuracy, precision, recall, F1-score, confusion matrix
- **Explainable AI:** Grad-CAM attention heatmaps for interpretable predictions

## Features

- **Automated image preprocessing and augmentation**
- **Custom class weighting** to address imbalance
- **Comparative evaluation** of multiple backbone models
- **Explainable AI (XAI):** Visual tumor-region heatmaps via Grad-CAM
- **Reproducible results:** Model checkpoints, training curves, confusion matrices

## Key Results

- **EfficientNetB0:** Achieved high validation accuracy and recall
- **Interpretability:** Grad-CAM heatmaps highlight clinically relevant areas for each prediction
- **Full benchmark:** Precision, recall, F1-score, ROC-AUC, per-class accuracy

## Project Structure

```
├── training_code.py           # Full model training pipeline
├── xai_gradcam.py             # Grad-CAM explainability scripts
├── outputs/                   # Saved model weights, result images, curves
├── README.md                  # Project overview and usage
```

## Usage

1. **Train Models**  
   - Run `training_code.py` to train VGG16, ResNet50, EfficientNetB0 on the MRI dataset (`/Training` and `/Testing`).
   - Models and plots are saved to `/outputs/`.

2. **Generate Grad-CAM Explanation**  
   - Run `xai_gradcam.py` after training to produce Grad-CAM heatmaps and overlay visualizations.

3. **View Results**  
   - Visualizations and model artifacts are in `/outputs/`.

## Highlights

- 🧠 **Computer vision classification** of medical MRI scans  
- 📈 **Accuracy, recall, F1** benchmarked for 4 classes  
- 🔍 **Grad-CAM**: See what regions the model focuses on for diagnosis  
- 👩‍⚕️ **Clinical utility**: Designed to enhance trust in AI-assisted diagnosis




