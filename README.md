# 📱 Mobile_Classifier

This project focuses on **image classification on mobile devices**, using a **lightweight Convolutional Neural Network (CNN)** to classify images of mobile phones from a custom dataset. The goal is to build an **efficient and accurate deep learning model** that can be deployed on smartphones or edge devices with limited computational power.

---

## 📌 Introduction

This project uses **deep learning** techniques to classify different **mobile phone brands** from image data. The model is built using **Keras** and **TensorFlow**, and is capable of distinguishing between popular brands such as:

- Apple
- Samsung
- Oppo
- Vivo
- Xiaomi

---

## 📁 Dataset

The dataset consists of labeled images organized in the following folder structure:
dataset/
├── Apple/
├── Samsung/
├── Oppo/
├── Vivo/
└── Xiaomi/


Each folder contains images corresponding to that specific brand.

---

## ⚙️ Data Preprocessing

- Images were resized to **224x224** pixels.
- **Data Augmentation** was applied using `ImageDataGenerator`, including:
  - Rotation
  - Flipping
  - Zooming
  - Brightness adjustment
- All pixel values were **normalized** to the range `[0, 1]`.

---

## 🧠 Model Architecture

The CNN architecture includes:
- `Conv2D` layers with **ReLU** activation
- `MaxPooling2D` layers to reduce spatial dimensions
- `Dropout` layers to prevent overfitting
- `Dense` layers followed by a **Softmax** output for multi-class classification

### 🛠 Compilation Details
- **Loss Function**: `categorical_crossentropy`
- **Optimizer**: `Adam`
- **Metrics**: `accuracy`

---

## 📊 Training Details

- Trained for **15–25 epochs** using training and validation splits.
- Model performance monitored using:
  - Training & Validation **Accuracy**
  - Training & Validation **Loss**
- **Confusion Matrix** plotted to analyze classification performance.

---

## ✅ Results

The trained model achieved **high validation accuracy**. Performance was evaluated using:
- Accuracy
- Loss
- Confusion Matrix

---

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Mobile_Classifier.git
   cd Mobile_Classifier


