# 🧬 Explainability-Guided Colon Cancer Detection

Deep learning-based colon cancer detection using EfficientNetB0 with Grad-CAM explainability and K-Fold cross-validation.

---

## 📌 Overview

This project presents an AI-driven approach for detecting colon cancer from histopathological images. It combines a high-performance convolutional neural network with explainable AI techniques to improve both prediction accuracy and interpretability.

The system classifies images as *Cancer* or *Normal* and highlights key regions influencing predictions using Grad-CAM, making it suitable for real-world medical decision support.

---

## 🎯 Objectives

* Build a robust deep learning model for colon cancer detection
* Improve generalization using K-Fold Cross Validation
* Provide visual explanations for predictions
* Enable real-time testing via an interactive interface

---

## 🚀 Key Features

* EfficientNetB0-based transfer learning model
* Grad-CAM heatmap visualization
* 5-Fold Cross Validation for robustness
* Real-time prediction using Gradio UI
* Balanced dataset training

---

## 🧠 Model Architecture

* **Backbone:** EfficientNetB0 (pretrained on ImageNet)
* **Input Shape:** 224 × 224 × 3
* **Output:** Binary Classification (Cancer / Normal)
* **Loss Function:** Binary Crossentropy
* **Optimizer:** Adam / AdamW
* **Activation:** Sigmoid

---

## 📊 Dataset

* **Dataset:** LC25000
* **Total Images:** 10,000

  * 5,000 Colon Adenocarcinoma
  * 5,000 Normal Colon Tissue

> Dataset not included due to size constraints.

---

## 📈 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Specificity
* ROC-AUC
* Precision–Recall Curve

---

## 🔍 Explainability (Grad-CAM)

Grad-CAM (Gradient-weighted Class Activation Mapping) is used to visualize regions that influence model predictions.

Benefits:

* Improved model transparency
* Better interpretability for medical use
* Easier debugging of model behavior

---

## 🖥️ Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Gradio

---

## 📁 Project Structure

```
Explainability-Colon-Cancer/
│
├── notebooks/
│   └── training.ipynb
│
├── src/
│   ├── model.py
│   ├── gradcam.py
│   └── utils.py
│
├── app/
│   └── gradio_app.py
│
├── results/
│   ├── plots/
│   └── outputs/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🧪 Results

* Achieved strong classification performance on validation data
* Consistent results across 5-fold cross-validation
* High-quality Grad-CAM visual explanations
* Stable ROC-AUC and Precision–Recall curves

---

## 📌 Future Enhancements

* Multi-class cancer classification
* Deployment using Flask/Streamlit
* Integration with clinical workflows
* Optimization for edge devices

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

---

## 👨‍💻 Author

**N LAVANKUMAR**

---
