# Audio Deepfake Detection

This project implements an audio deepfake detection system using deep learning. Three different approaches were explored:

1. **CNN with MFCC Features**
2. **ResNet with Mel-Spectrogram Features**
3. **Graph Attention Network (GAT)**

---

## Overview

For our analysis, we focus on the **ResNet with Mel-Spectrogram Features** approach. In this model:
- Audio files are converted into mel-spectrograms.
- A modified ResNet18 (with the first convolution adjusted for a single-channel input) extracts deep hierarchical features.
- The final layers output a binary classification, distinguishing genuine (bonafide) from spoofed audio.

---

## How to Run

Simply run the main training script to preprocess the data, train the model, and evaluate its performance. The script outputs training/validation metrics along with a confusion matrix for analysis.

---

## Analysis

The ResNet approach was chosen due to its:
- **Effective Feature Extraction:** Captures complex time-frequency patterns from mel-spectrograms.
- **Robust Performance:** Demonstrated high accuracy and strong discrimination between genuine and AI-generated speech.
- **Balanced Trade-off:** Offers an optimal balance between computational efficiency and detection capability.

---

## Future Work

- Enhance data augmentation techniques.
- Fine-tune hyperparameters for improved performance.
- Optimize for real-time deployment.
