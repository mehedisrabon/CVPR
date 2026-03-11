Here is a professional and structured `README.md` file for your GitHub repository. It organizes your five assignments into a cohesive "Computer Vision & Deep Learning Portfolio," highlighting the progression from foundational algorithms to advanced transfer learning.

---

# Computer Vision & Deep Learning Portfolio

This repository contains a series of assignments exploring the evolution of Computer Vision (CV) and Machine Learning (ML) techniques—starting from fundamental algorithms built with NumPy to deploying real-time biometric systems using State-of-the-Art (SOTA) Deep Learning architectures.

## 🚀 Project Overview

The portfolio is divided into five key milestones, each focusing on a different aspect of image classification, neural architecture, and real-time inference.

### 1. Fundamental Image Classification (k-NN)

Developed a k-Nearest Neighbors (k-NN) classifier from scratch to categorize images of cats, dogs, and pandas.

* **Key Features:** Manual implementation of L1 (Manhattan) and L2 (Euclidean) distance metrics.
* **Analysis:** Used 5-fold cross-validation to determine the optimal $k$-value and analyzed the performance trade-offs between different distance functions.

### 2. Neural Networks from Scratch

Designed and implemented a Multi-Layer Perceptron (MLP) with three hidden layers ($64 \rightarrow 32 \rightarrow 16$) using only NumPy.

* **Optimization:** Built the backpropagation algorithm, Xavier weight initialization, and mini-batch gradient descent manually.
* **Activation:** Utilized ReLU for hidden layers and Softmax with Categorical Cross-Entropy for multi-class classification (5 classes).

### 3. Real-Time Digit Recognition Pipeline

Bridged the gap between static training and real-world data by creating an end-to-end MNIST digit recognizer.

* **Preprocessing:** Built a custom OpenCV pipeline featuring adaptive thresholding, morphological noise reduction, and center-of-mass alignment.
* **Inference:** Integrated a JavaScript-webcam bridge to perform real-time classification on handwritten digits captured live.

### 4. CNN-Based Face Attendance System

Implemented a biometric system to automate attendance through facial recognition.

* **Dataset:** Engineered a custom facial dataset with person-specific labels.
* **Logic:** Developed a CNN classifier that triggers an "Attendance Marked" event only when a 70% confidence threshold is met, ensuring system reliability against false positives.

### 5. Advanced Biometrics with Transfer Learning (ResNet50)

Leveraged industry-standard Transfer Learning to enhance the accuracy and robustness of the facial recognition system.

* **Architecture:** Integrated the **ResNet50** backbone (pre-trained on ImageNet) and fine-tuned it for facial identification.
* **Efficiency:** Achieved superior convergence speed and accuracy by utilizing high-dimensional feature maps from a deep residual network.

---

## 🛠️ Tech Stack

* **Languages:** Python, JavaScript (for webcam integration)
* **Libraries:** NumPy, TensorFlow, Keras, OpenCV, Matplotlib, Scikit-learn
* **Environments:** Google Colab, Google Drive (for model persistence)

## 📊 Key Results

* **k-NN:** Comparative analysis of L1 vs L2 distances across multiple $k$ hyperparameters.
* **Neural Net:** Achieved **~99.6% accuracy** on synthetic 5-class Gaussian clusters.
* **ResNet50:** High-precision real-time identification with robust performance under varying lighting conditions.

## 📂 Repository Structure

```text
├── MID/
│   ├── Assignment_1_kNN.ipynb             # k-Nearest Neighbors from scratch
│   ├── Assignment_2_NN_Scratch.ipynb      # Neural Network backprop from scratch
├── Final/
│   ├── Digit Detection/
│   │   ├── demoMNIST.ipynb                # Real-time digit recognition pipeline
│   │   ├── digit.ipynb                    # MNIST model training logic
│   ├── CNN-Based Face Attendance System/  # Custom CNN for biometric logging
│   └── Advanced Biometrics with Transfer Learning (ResNet50)/ # SOTA face identification
└── README.md

```

---

*Developed as part of the Computer Vision & Pattern Recognition (CVPR) Coursework.*