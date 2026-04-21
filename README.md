# 🧬 Explainability-Guided Colon Cancer Detection

Deep learning-based colon cancer detection using EfficientNetB0 with Grad-CAM explainability and K-Fold cross-validation.

---

## 📌 Overview

This project presents an AI-driven approach for detecting colon cancer from histopathological images. It combines a high-performance convolutional neural network with explainable AI techniques to improve both prediction accuracy and interpretability.

The system classifies images as *Cancer* or *Normal* and highlights key regions influencing predictions using Grad-CAM, making it suitable for real-world medical decision support.

---

## 📖 Extended Description

Colon cancer is one of the leading causes of cancer-related deaths worldwide, and early detection plays a crucial role in improving survival rates. Traditional diagnosis through histopathological analysis is time-consuming and depends heavily on expert interpretation.

This project introduces an end-to-end deep learning pipeline using EfficientNetB0 for feature extraction and classification. To ensure robustness, 5-Fold Cross Validation is applied, reducing overfitting and improving generalization.

A key highlight is the integration of Explainable AI using Grad-CAM, which provides visual explanations by highlighting important regions in the image that influence predictions. This improves transparency and trust, especially in medical applications.

Additionally, a Gradio-based interface is developed for real-time image testing, enabling users to upload images and visualize predictions along with heatmaps.

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

* **Dataset:** LC25000 (Histopathological Image Dataset)
* Contains thousands of labeled histopathology images including colon adenocarcinoma and benign tissue classes ([Kaggle][1])

🔗 Dataset Link: https://www.kaggle.com/datasets/andrewmvd/colorectal-histology-dataset

> Note: Dataset is not included in this repository due to size limitations.

---

## 📥 Dataset Setup

1. Download dataset from the above link
2. Extract and organize as follows:

```
data/
 ├── train/
 ├── test/
```

---

## 📸 Application Demo

### 🔹 Upload Interface

![Upload UI](https://github.com/NLavanKumar/Explainability-Guided-Colon-Cancer-Detection/blob/main/images/gradio_upload_screen.png)

### 🔹 Cancer Prediction with Grad-CAM

![Cancer Output](https://github.com/NLavanKumar/Explainability-Guided-Colon-Cancer-Detection/blob/main/images/prediction_cancer_result.png)

### 🔹 Normal Tissue Prediction

![Normal Output](https://github.com/NLavanKumar/Explainability-Guided-Colon-Cancer-Detection/blob/main/images/prediction_normal_result.png)

### 🔹 Full Application Interface

![App Interface](https://github.com/NLavanKumar/Explainability-Guided-Colon-Cancer-Detection/blob/main/images/gradio_app_interface.png)

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
├── data/
│   └── (dataset should be placed here)
│
├── results/
│   ├── plots/
│   └── outputs/
│
├── images/
│   └── (screenshots used in README)
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

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
python app/gradio_app.py
```

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

**N Lavankumar**

---

[1]: https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images?utm_source=chatgpt.com "Lung and Colon Cancer Histopathological Images"
