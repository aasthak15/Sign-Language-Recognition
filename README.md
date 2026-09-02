# 🤟 Sign Language Recognition Using Computer Vision & Deep Learning

<p align="center">
  <strong>An AI-powered system for recognizing sign language gestures using Computer Vision and Deep Learning.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python">
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv">
  <img src="https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange?logo=tensorflow">
  <img src="https://img.shields.io/badge/Keras-Neural%20Networks-red?logo=keras">
  <img src="https://img.shields.io/badge/Domain-Artificial%20Intelligence-purple">
</p>

---

## 📌 Project Overview

Sign language is an important means of communication for people with hearing and speech impairments. However, communication between sign language users and people unfamiliar with sign language can be difficult.

This project aims to bridge this communication gap by developing a **computer vision and deep learning based Sign Language Recognition System**.

The system captures hand gestures through a camera, processes the captured image using OpenCV, extracts the relevant Region of Interest (ROI), and uses a trained Convolutional Neural Network (CNN) to classify the gesture.

The recognized sign can then be used as the foundation for a larger **sign-to-text or sign-to-speech communication system**.

---

# 🎯 Objectives

The major objectives of this project are:

- To develop an automated sign language recognition system.
- To capture hand gestures using a camera.
- To identify the relevant hand region using computer vision techniques.
- To preprocess the captured image for classification.
- To use a Convolutional Neural Network for gesture classification.
- To recognize different sign language alphabet gestures.
- To provide a foundation for real-time sign language communication.
- To explore the application of Artificial Intelligence in assistive technologies.

---

# ✨ Key Features

### 📷 Real-Time Image Capture

The system can capture hand gestures using a camera and process the input image for recognition.

### 🖐️ Region of Interest Detection

OpenCV is used to identify and process the relevant region of the image containing the hand gesture.

### 🧹 Image Preprocessing

The captured image is prepared before being passed to the neural network. Preprocessing helps improve the quality and consistency of the input.

### 🧠 CNN-Based Classification

A Convolutional Neural Network is used to learn visual features from hand gesture images and classify them into the corresponding sign classes.

### 🔤 Sign Recognition

The system is designed to recognize hand signs corresponding to alphabetic gestures using a trained deep learning model.

### ⚡ Real-Time Processing

The OpenCV pipeline allows the system to process camera input interactively.

---

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV | Image processing and computer vision |
| TensorFlow | Deep learning framework |
| Keras | CNN model development |
| NumPy | Numerical and array operations |
| Google Colab | Model training and experimentation |
| Jupyter Notebook | Model development and testing |
| Git & GitHub | Version control and project management |


---

# 📊 Dataset

The project uses the **Sign Language MNIST dataset**, which contains images of hand gestures representing American Sign Language (ASL) alphabet classes.

### Dataset Source

[Kaggle – Sign Language MNIST](https://www.kaggle.com/datamunge/sign-language-mnist)

### Dataset Characteristics

- Grayscale hand gesture images
- Standardized image dimensions
- Multiple ASL alphabet classes
- Training and testing data
- Suitable for CNN-based image classification

The dataset is used to train and evaluate the deep learning model for sign classification.

---

# 📁 Project Structure

```text
Sign-Language-Recognition/
│
├── ASL.ipynb
├── ASL2.ipynb
├── ASLwithCNN.ipynb
├── CNNmodel.h5
├── HandHisto.py
├── ISL.py
├── LICENSE
├── README.md
├── ROIinOpenCV.py
├── _config.yml
├── cnn.py
├── islpaper.pdf
├── model.h5
├── model_weights.h5
├── opencv.py
├── requirements.txt
└── sign_language_pytorch.ipynb
```



# 🏗️ System Architecture

The overall workflow of the system can be represented as:

```text
              ┌─────────────────────┐
              │      Camera         │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │   Image Capture     │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │  ROI Detection      │
              │   using OpenCV      │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Image Preprocessing │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │   CNN / Deep        │
              │   Learning Model    │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Gesture Prediction  │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Recognized Sign /   │
              │ Alphabet            │
              └─────────────────────┘

```





# 🧠 CNN Model Architecture

The system uses a **Convolutional Neural Network (CNN)** for classifying hand gesture images.

The CNN learns visual features automatically from the input images.

### Model Pipeline

```text
Input Image
     ↓
Convolution Layer
     ↓
Activation Function
     ↓
Pooling Layer
     ↓
Convolution Layer
     ↓
Pooling Layer
     ↓
Flatten
     ↓
Fully Connected Layer
     ↓
Output Layer
     ↓
Predicted Sign


