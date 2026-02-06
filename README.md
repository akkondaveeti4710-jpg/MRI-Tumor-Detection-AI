# MRI Tumor Detection AI

## AI-Assisted Brain Tumor Detection Using MRI and Explainable Deep Learning

---

## Overview

This project develops a deep learning system to classify brain MRI scans into four categories: **glioma, meningioma, pituitary tumor, and no tumor.** The system uses a Convolutional Neural Network (CNN) combined with Grad-CAM explainability to support transparent AI-assisted screening.

The broader goal is to explore how AI can improve **healthcare accessibility**, particularly in rural or underserved regions where neuroradiology expertise is limited. The model is designed as a *screening aid*, not a diagnostic replacement.

---

## Motivation

Brain tumor diagnosis requires trained neuroradiologists and advanced imaging facilities. Many regions worldwide lack access to such specialists due to geographic and socioeconomic barriers. AI systems that assist preliminary MRI interpretation could help reduce diagnostic delays and support equitable healthcare delivery.

This project investigates whether deep learning can provide accurate and interpretable tumor classification from MRI scans.

---

## Dataset

This project uses the publicly available **Brain MRI Images Dataset (Kaggle).**

### Class Distribution

- Glioma — 826 images  
- Meningioma — 822 images  
- Pituitary — 827 images  
- No Tumor — 395 images  

### Preprocessing

- All images resized to **224 × 224**  
- Pixel normalization applied  
- Dataset split into **80% training / 20% validation**  
- Data shuffled to reduce bias

---

## Model Architecture

A Convolutional Neural Network (CNN) was implemented using TensorFlow/Keras.

The architecture includes:

- Convolutional layers for feature extraction  
- Max-pooling layers for dimensionality reduction  
- Dense layers for classification  
- Softmax output layer for multi-class prediction

---

## Training Details

- **Optimizer:** Adam  
- **Loss Function:** Categorical Cross-Entropy  
- **Epochs:** 10–20  
- **Batch Size:** 32  
- **Learning Rate:** 0.001  
- **Hardware:** Google Colab GPU

---

## Performance

| Metric | Value |
|--------|------|
| Training Accuracy | ~96% |
| Validation Accuracy | ~95% |

### Robustness Test

To simulate real-world conditions, lower-quality MRI images were tested.

- Accuracy drop observed: **8–12%**  
- Indicates sensitivity to scan quality

---

## Explainability

Grad-CAM (Gradient-weighted Class Activation Mapping) was applied to visualize regions influencing predictions. Heatmaps frequently aligned with tumor regions, suggesting meaningful feature learning.

Explainability increases transparency and trust, which are essential for medical AI.

---

## Applications

Potential uses include:

- AI-assisted screening  
- Educational tools  
- Telemedicine support  
- Preliminary triage in low-resource settings

---

## Limitations

- Dataset may not reflect full clinical diversity  
- No clinical validation performed  
- Not approved for medical diagnosis  
- AI cannot replace trained physicians

This system should be used only as a research or educational tool.

---

## Ethical Considerations

Responsible AI use requires:

- Patient data privacy  
- Medical supervision  
- Avoiding over-reliance on AI  
- Transparency in predictions

AI should support clinicians, not replace them.

---

## Future Work

Future improvements may include:

- Larger and more diverse datasets  
- Multi-hospital validation  
- Clinical testing with experts  
- Improved robustness to image quality  
- Deployment for telemedicine support

---

## How to Run

1. Clone the repository  
2. Open the notebook in Google Colab
3. Run all cells  
4. Upload MRI images for prediction

---

## Citation

If you use this work, please cite:

**Kondaveeti, A. (2026).** *MRI Tumor Detection AI* [Computer software]. GitHub.  
https://github.com/akkondaveeti4710-jpg/MRI-Tumor-Detection-AI

---

## License

For academic and research use only.

4. Install dependencies  

