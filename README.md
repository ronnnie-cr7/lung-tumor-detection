# 🫁 Lung Tumor Segmentation using 3D U-Net (Deep Learning Project)

## 📌 Project Overview

This project focuses on **automated lung tumor segmentation** from 3D CT scan data using deep learning techniques. The goal is to accurately identify tumor regions, which can assist in early diagnosis and treatment planning.

The project is divided into three major stages:

1. Exploratory Data Analysis (EDA)
2. Baseline 3D U-Net Model Implementation
3. Performance Enhancement using Data Augmentation

---

## 🎯 Objectives

* Analyze and understand CT scan datasets
* Implement a **3D U-Net architecture** for medical image segmentation
* Evaluate segmentation performance using **Dice Score**
* Improve model generalization using **data augmentation**
* Compare baseline and improved models

---

## 📂 Project Structure

```
lung-tumor-detection/
│
├── M1_EDA_Analysis.ipynb
├── M2_3D_UNet_Segmentation.ipynb
├── M3_Data_Augmentation_Comparison.ipynb
└── README.md
```

---

## 🔍 Detailed Workflow

### 🔹 M1: Exploratory Data Analysis (EDA)

* Visualized CT scan slices
* Identified tumor vs non-tumor regions
* Checked class imbalance and data distribution
* Performed preprocessing (normalization, resizing if applicable)

---

### 🔹 M2: 3D U-Net Model for Segmentation

* Implemented **3D U-Net architecture** for volumetric data
* Used encoder-decoder structure with skip connections
* Trained model on CT scan volumes
* Evaluated performance using:

👉 **Dice Score (Segmentation Metric)**

* Measures overlap between predicted and ground truth masks
* Higher value = better segmentation accuracy

---

### 🔹 M3: Data Augmentation & Model Comparison

* Applied augmentation techniques:

  * Rotation
  * Flipping
  * Scaling
* Improved dataset diversity
* Compared:

  * Baseline 3D U-Net
  * Augmented Model
* Observed improvement in generalization and Dice Score

---

## 📊 Results & Insights

* Baseline model provided reasonable segmentation performance
* Data augmentation significantly improved:

  * Model robustness
  * Generalization on unseen data
* Dice Score comparison demonstrates effectiveness of augmentation

---

## 📁 Dataset

* 📌 Dataset Link: https://www.kaggle.com/datasets/zhangweiled/lidcidri/data
* Source: Kaggle / Medical dataset repository

⚠️ Note: Dataset is not included due to large size.

---

## 🛠️ Tech Stack

* Python
* Deep Learning (TensorFlow / PyTorch)
* NumPy, OpenCV
* Matplotlib / Seaborn
* Google Colab (for training)

---

## ⚙️ How to Run the Project

1. Clone the repository:

   ```
   git clone https://github.com/your-username/lung-tumor-detection.git
   ```
2. Open notebooks in Google Colab
3. Update dataset path
4. Run all cells step-by-step

---

## 📈 Future Improvements

* Use advanced architectures (Attention U-Net, UNet++)
* Hyperparameter tuning
* Deploy as a web app (Streamlit)
* Integrate real-time medical imaging pipeline

---

## 📚 References
https://www.sciencedirect.com/science/article/pii/S1746809423010832

---

## 👨‍💻 Author

Ronit
