# 🩺 Skin Disease Classification Using CNN and the HAM10000 Dataset

This project implements a Convolutional Neural Network (CNN) to classify skin lesions using dermatoscopic images from the **HAM10000** dataset. The goal is to support early detection of skin conditions like melanoma by automating image-based classification.

---

## 📁 Dataset

**HAM10000 ("Human Against Machine with 10000 training images")**  
A publicly available dataset containing 10,000 dermatoscopic images of pigmented skin lesions across 7 classes:

- `akiec` — Actinic keratoses
- `bcc` — Basal cell carcinoma
- `bkl` — Benign keratosis-like lesions
- `df` — Dermatofibroma
- `mel` — Melanoma
- `nv` — Melanocytic nevi
- `vasc` — Vascular lesions

📝 Dataset source: [Kaggle - HAM10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)

---

## 🧠 Model Overview

We designed a custom CNN architecture from scratch using TensorFlow/Keras. Key steps include:

- Image resizing and normalization (96×96)
- Label encoding and one-hot transformation
- Data augmentation (rotation, zoom, shift, flip)
- CNN with 2 Conv layers, MaxPooling, Dropout, and Softmax output
- Train-test split (80/20) with validation metrics

---

## 🔍 Evaluation

- Final test accuracy: ~76%
- Strong performance on majority class (`melanocytic nevi`)
- Confusion matrix and classification report used for in-depth evaluation

⚠️ Observed class imbalance, which affected rare class predictions.

---

## 📈 Visuals

- Accuracy/loss plots across epochs
- Confusion matrix to show per-class performance

---
