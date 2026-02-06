# MRI-Tumor-Detection-AI
AI model for brain tumor detection using MRI and explainable AI

# MRI Brain Tumor Detection using Deep Learning

## Overview
This project uses a Convolutional Neural Network (CNN) to detect brain tumors from MRI scans.  
The model classifies images into:
- Glioma
- Meningioma
- Pituitary
- No Tumor

Grad-CAM visualizations are used to explain model decisions.

## Features
- MRI tumor classification
- Grad-CAM explainability
- High accuracy (~95%)
- Clean training pipeline

## Tech Stack
- Python
- TensorFlow / Keras
- Google Colab
- Grad-CAM visualization

## Results
- Training Accuracy: ~95%
- Validation Accuracy: ~95%
- Explainable AI heatmaps included

## Note
Model file not uploaded due to GitHub size limits. Available upon request.

This project uses the Brain MRI Images dataset from Kaggle:
- Glioma: 826 images
- Meningioma: 822 images
- Pituitary: 827 images
- No Tumor: 395 images
  
Images were resized to 224x224, normalized, and split into 80% training / 20% validation.

## How to Run
1. Clone repo
2. Open notebook in Google Colab
3. Install requirements: `pip install -r requirements.txt`
4. Run cells
5. Upload your MRI image

## Model Performance
- Training accuracy: 96%
- Validation accuracy: 95%

## Performance on low-quality images
- Accuracy drop: ~8-12%

## Explainability
Grad-CAM was used to interpret model decisions. Heatmaps are generated from intermediate layers to highlight the regions influencing predictions, providing transparency and clinical relevance.

## Citation
If you use this work in a research project, please cite as:

Kondaveeti, A. (2026). MRI Tumor Detection AI [Source code]. Github repository.
https://github.com/akkondaveeti4710-jpg/MRI-Tumor-Detection-AI
