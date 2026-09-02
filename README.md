# Garbage-Classification
# ♻️ Garbage Classification Using Deep Learning

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.X-orange.svg)](https://www.tensorflow.org/)
[![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-yellow.svg)](https://ultralytics.com/)
[![Google Colab](https://img.shields.io/badge/Google-Colab-orange.svg)](https://colab.research.google.com/)

---

## 📌 Project Overview

This project focuses on **multi-class waste image classification** using Deep Learning techniques. 

Three different architectures were implemented, trained, and compared throughout the project:
* **CNN (Baseline Model)** – Custom built from scratch.
* **MobileNetV2 (Transfer Learning)** – Pretrained ImageNet weights.
* **YOLOv8-cls (Ultralytics Classification)** – Modern classification model.

The objective is to determine which model provides the best balance between **classification accuracy**, **computational efficiency**, and **real-world usability**.

---

## 🎯 Project Objectives

* Build a baseline Convolutional Neural Network (CNN) from scratch.
* Apply Transfer Learning using MobileNetV2.
* Train an image classification model using YOLOv8-cls.
* Compare all models under identical evaluation criteria (Accuracy, Precision, Recall, F1-Score).
* Measure computational efficiency using model size, parameter count, and inference time.

---

## 📁 Dataset

* **Source:** Kaggle – Garbage Classification Dataset
* **Classes (6):** Cardboard, Glass, Metal, Paper, Plastic, Trash.
* **Image Resolution:** 224 × 224 RGB.
* **Data Split:** Train (~70%), Validation (~15%), Test (~15%).

---

## 🧠 Deep Learning Models & Performance

The three models were evaluated using the test dataset and compared based on accuracy and speed:

| Model | Accuracy (%) | Model Size | Inference Time |
| :--- | :---: | :---: | :---: |
| 🥇 **YOLOv8-cls** | **80.00%+** | 6.2 MB | 24.71 ms |
| 🥈 **MobileNetV2** | **77.78%** | 14.2 MB | 216.58 ms |
| 🥉 **CNN (Baseline)** | **39.29%** | ~2.5 MB | 90.12 ms |

---

## 🛠️ Technologies & Libraries

* Python
* TensorFlow / Keras
* Ultralytics YOLOv8
* NumPy & Pandas
* Matplotlib / Seaborn
* Scikit-learn
* Google Colab

---

## 📂 Project Structure

```text
Garbage_Classification_DeepLearning/
│
├── app/
│   └── Garbage_Classification_DeepLearning.ipynb  # Colab Notebook
│
├── data/
│   └── dataset/                                   # Garbage Classification Dataset
│
├── models/
│   ├── basit_cnn_atik_modeli.keras                # Saved CNN Model
│   ├── mobilenetv2_atik_modeli.keras              # Saved MobileNetV2 Model
│   └── best.pt                                    # Saved YOLOv8 Weights
│
└── README.md
