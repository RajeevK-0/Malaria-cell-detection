# Malaria Cell Detection using CNN

## 📌 Project Overview
This project implements a Convolutional Neural Network (CNN) to detect malaria-parasitized cells in thin blood smear images. Malaria is a life-threatening disease caused by parasites transmitted to people through the bites of infected female Anopheles mosquitoes. Early and accurate detection is crucial for effective treatment.

This solution automates the diagnosis process by classifying cell images as either **Parasitized** or **Uninfected** with high accuracy, leveraging Deep Learning techniques.

## 🚀 Key Features
* **Custom CNN Architecture:** A deep learning model built from scratch using Keras/TensorFlow.
* **Data Preprocessing:** Automated image resizing (64x64), normalization, and label encoding.
* **Performance Visualization:** Matplotlib graphs to track accuracy and loss over training epochs.
* **Robust Training:** Utilizes Batch Normalization and Dropout layers to prevent overfitting.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Deep Learning:** TensorFlow, Keras
* **Computer Vision:** OpenCV, PIL (Pillow)
* **Data Handling:** NumPy, Pandas
* **Visualization:** Matplotlib

## 📂 Dataset
The project utilizes the Malaria Cell Images Dataset (commonly available on Kaggle/NIH).
* **Classes:** 2 (Parasitized, Uninfected)
* **Input Shape:** 64x64x3 (RGB images)

## 🧠 Model Architecture
The model consists of a sequential CNN architecture:
1.  **Convolutional Blocks:** Two blocks containing Conv2D (32 filters), MaxPooling, BatchNormalization, and Dropout.
2.  **Flatten Layer:** Converts 2D feature maps to 1D vectors.
3.  **Dense Layers:** Fully connected layers with ReLU activation for feature classification.
4.  **Output Layer:** Sigmoid activation for binary classification.

## 📊 Results
The model evaluates the test set to determine generalization performance.
*(Note: You can update this section with your specific accuracy numbers after running the final training, e.g., "Achieved 95% Accuracy on the test set.")*

## 🔧 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/malaria-cell-detection.git](https://github.com/yourusername/malaria-cell-detection.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install tensorflow pandas numpy matplotlib opencv-python tqdm
    ```
3.  **Update Data Path:**
    Open the script and update the `img_dir` variable to point to your local dataset location.
4.  **Run the script:**
    ```bash
    python malariacelldetection.py
    ```
