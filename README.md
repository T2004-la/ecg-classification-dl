# 🫀 ECG Signal Classification using Deep Learning

This repository contains a Python implementation for processing and classifying Electrocardiogram (ECG) signals using TensorFlow/Keras and Deep Neural Networks. The project processes time-series ECG data to classify heart signals into **Normal** and **Abnormal** categories.

## 📌 Project Overview
- **Domain:** Medical Signal Processing & Healthcare AI
- **Model Architecture:** Deep Neural Network (Sequential / Dense Layers with Dropout)
- **Frameworks & Libraries:** TensorFlow, Keras, NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn
- **Objective:** Automated binary classification of ECG heartbeat signals.

## 📊 Dataset Information
The project is designed to work with the **PTB Diagnostic ECG Database**:
- `ptbdb_normal.csv`: ECG signals from healthy control subjects.
- `ptbdb_abnormal.csv`: ECG signals from patients with various heart conditions.

> **Note:** The script includes an automated fallback mechanism that generates synthetic time-series data if the raw CSV files are not detected in the working directory, ensuring seamless pipeline execution.

## 🛠️ Project Structure & Workflow
1. **Data Loading & Validation:** Checks for local dataset files or generates synthetic sequence data.
2. **Preprocessing:** Feature normalization using `StandardScaler` and stratified data splitting (`train_test_split`).
3. **Neural Network Construction:** Multi-layer Perceptron (MLP) architecture built with Keras.
4. **Model Evaluation:** Computes accuracy, loss, confusion matrix, and ROC-AUC curves.

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/T2004-la/ecg-classification-dl.git](https://github.com/T2004-la/ecg-classification-dl.git)
   cd ecg-classification-dl