

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

## 📁 Dataset & Class Distribution

* **Source:** Kaggle – Garbage Classification Dataset
* **Image Resolution:** 224 × 224 RGB
* **Data Split:** Train (~70%), Validation (~15%), Test (~15%)

### Classes & Sample Distribution:
| Class Name | Description & Visual Contents | Image Count |
| :--- | :--- | :---: |
| 📦 **Cardboard** | Corrugated boxes, packaging cartons, brown paper containers | **806** |
| 🍾 **Glass** | Glass bottles, jars, broken glass fragments | **1,002** |
| 🔩 **Metal** | Aluminum cans, metal tins, scrap metals | **820** |
| 📄 **Paper** | Office paper, newspapers, magazines, notebooks | **1,188** |
| 🥤 **Plastic** | Plastic bottles, containers, wrappers, disposable cups | **964** |
| 🗑️ **Trash** | Mixed general waste, non-recyclable debris | **274** |

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

## 🚀 Conclusion & Industrial Recommendation

* **YOLOv8-cls** achieved the highest accuracy, smallest size, and fastest inference time, making it the most suitable model for real-time industrial waste sorting on conveyor belts.
* **MobileNetV2** performed well as a secondary option via Transfer Learning.
* **Baseline CNN** served as a reference model but showed limitations due to its shallow architecture.
