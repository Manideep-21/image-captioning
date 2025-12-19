# Image Captioning using PyTorch

This project implements an **Image Captioning system** that automatically generates natural language descriptions for images using deep learning.  
The model follows an **Encoder–Decoder architecture**, implemented entirely in **PyTorch**.

---

## Overview
- **Task**: Image Captioning
- **Architecture**: CNN + LSTM (Encoder–Decoder)
- **Framework**: PyTorch
- **Platform**: Kaggle Notebook

---

## Model Architecture

### Encoder (CNN)
- Pretrained Convolutional Neural Network
- Extracts high-level visual features from images
- Outputs a fixed-length feature vector

### Decoder (LSTM)
- Word embedding layer
- LSTM network for sequence generation
- Fully connected layer with Softmax for next-word prediction

---

## Dataset & Preprocessing
- Image–caption dataset
- Text preprocessing:
  - Lowercasing
  - Removing punctuation
  - Tokenization
  - Vocabulary creation
  - Padding sequences
- Image preprocessing:
  - Resizing
  - Normalization

---

## Training
- Loss Function: Cross-Entropy Loss
- Optimizer: Adam
- Trained using teacher forcing

---

## How to Run
1. Open `image-captioning.ipynb`
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
