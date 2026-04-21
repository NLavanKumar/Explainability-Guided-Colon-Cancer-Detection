# Explainability-Guided Colon Cancer Detection

Deep learning-based colon cancer detection using EfficientNetB0 with Grad-CAM explainability and K-Fold cross-validation.

---

## 📌 Project Overview
This project focuses on automated colon cancer detection using histopathological images. It combines deep learning with explainable AI techniques to provide both accurate predictions and visual interpretation of model decisions.

---

## 🚀 Features
- EfficientNetB0-based classification
- Grad-CAM visualization for explainability
- 5-Fold Cross Validation for robustness
- GUI for real-time image testing
- High classification accuracy

---

## 🧠 Model Details
- Backbone: EfficientNetB0
- Input Size: 224 × 224 × 3
- Output: Binary Classification (Cancer / Normal)
- Loss Function: Binary Crossentropy
- Optimizer: Adam / AdamW

---

## 📊 Dataset
- Dataset: LC25000
- Total images used: 10,000
  - 5,000 Colon Adenocarcinoma (Cancer)
  - 5,000 Normal Colon Tissue

---

## 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Specificity
- ROC Curve & AUC
- Precision–Recall Curve

---

## 🖥️ Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Gradio

---

## 💡 Explainability
Grad-CAM is used to highlight important regions in histopathological images that influence model predictions, improving interpretability and clinical trust.

---

## 🧪 Results
- Achieved near-perfect classification performance
- Strong ROC and Precision–Recall curves
- Stable performance across all 5 folds
- Effective visualization using Grad-CAM

---

## 📌 Future Work
- Evaluation on real clinical datasets
- Multi-class cancer classification
- Deployment as a web-based application

---

⭐ If you found this project useful, consider giving it a star!
