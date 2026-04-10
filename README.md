# Neuro-LiteNet-model
Neuro-LiteNet is a state-of-the-art, edge-optimized deep learning framework specifically engineered for the high-precision classification of brain tumors from MRI scans. Developed as a lightweight alternative to computationally heavy architectures like VGG-16 and ResNet-50, it achieves a superior 98% F1-score while maintaining a significantly smaller memory footprint.

# Neuro-LiteNet: Edge-Optimized Brain Tumor Classification
**Accuracy: 98% | F1-Score: 0.98 | Architecture: EfficientNetB0**

## Overview
Neuro-LiteNet is a lightweight deep learning framework designed for real-time brain tumor classification from MRI scans. Unlike heavy architectures (VGG16/ResNet), this model is optimized for edge deployment in clinical settings.

## Key Results
- **Precision/Recall:** 98% across all 4 classes (Glioma, Meningioma, Pituitary, No Tumor).
- **Explainable AI:** Integrated Grad-CAM to visualize tumor focus areas.
- **Efficiency:** ~4.5M parameters (80% smaller than VGG16).

## Visual Proof
### Training Performance
![Training History](visuals/training_history.png)

### Confusion Matrix
![Confusion Matrix](visuals/confusion_matrix.png)

### Grad-CAM Interpretability
![Grad-CAM](visuals/GradCAM_Result.png)

## Usage
python
import tensorflow as tf
model = tf.keras.models.load_model('model/Neuro_LiteNet_Final.h5')
# Ready for inference
