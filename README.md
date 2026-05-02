# 🫁 Lung Tumor Segmentation using 3D U-Net & Attention U-Net (Deep Learning Project)

---

## 📌 Project Overview

This project focuses on automated lung tumor segmentation from 3D CT scan volumes using deep learning techniques. The system aims to accurately identify tumor regions to support early diagnosis, treatment planning, and clinical decision-making.

The project evolves through multiple stages of improvement:

1. Exploratory Data Analysis (EDA)
2. Baseline 3D U-Net implementation
3. Performance improvement using data augmentation
4. Advanced segmentation using Attention U-Net
5. Uncertainty estimation using Monte Carlo Dropout
6. Evaluation using Dice Score and Hausdorff Distance

---

## 🎯 Objectives

- Analyze and understand 3D CT scan datasets
- Implement 3D U-Net for volumetric segmentation
- Improve generalization using data augmentation
- Enhance segmentation using Attention mechanisms
- Estimate prediction uncertainty using MC Dropout
- Evaluate performance using:
  - Dice Score (region overlap)
  - Hausdorff Distance (boundary accuracy)

---

## 📂 Project Structure

```
lung-tumor-detection/
│
├── M1_EDA_Analysis.ipynb
├── M2_3D_UNet_Segmentation.ipynb
├── M3_Data_Augmentation_Comparison.ipynb
├── M4_Lung_Tumor(1).ipynb
└── README.md
```

---

## 🔍 Detailed Workflow

### 🔹 M1: Exploratory Data Analysis (EDA)

- Visualized 3D CT scan slices (voxels)
- Identified tumor vs non-tumor regions
- Analyzed class imbalance
- Preprocessed volumetric data (normalization, reshaping)

---

### 🔹 M2: Baseline 3D U-Net Model

- Implemented 3D U-Net architecture
- Encoder–decoder structure with skip connections
- Input: 3D CT voxel volumes
- Output: tumor segmentation masks

Evaluation:
- Dice Score

---

### 🔹 M3: Data Augmentation

- Rotation, flipping, noise injection
- Improved generalization
- Reduced overfitting
- Increased Dice Score significantly

---

### 🔹 M4: Attention U-Net + MC Dropout

- Attention U-Net for focused tumor segmentation
- MC Dropout for uncertainty estimation
- Outputs:
  - Segmentation mask
  - Uncertainty map

---

## 📊 Evaluation Metrics

### Dice Score
Measures overlap between prediction and ground truth.

### Hausdorff Distance
Measures maximum boundary deviation between predicted and actual tumor.

### Uncertainty Map
Indicates model confidence per voxel.

---

## 📈 Results Summary

| Model | Dice Score | Insight |
|------|------------|--------|
| 3D U-Net | ~0.44 | Baseline performance |
| + Augmentation | ~0.65 | Strong improvement |
| Attention U-Net + MC Dropout | ~0.68–0.70 | Best performance + uncertainty |

---

## 🫁 Dataset

- LIDC-IDRI dataset (Kaggle)
- 3D CT scans with voxel-level annotations
- Binary segmentation (tumor / non-tumor)

---

## 🛠️ Tech Stack

- Python
- TensorFlow / PyTorch
- NumPy, OpenCV
- Matplotlib
- Google Colab

---

## 🚀 Future Improvements

- Dice + Focal loss
- HD95 metric integration
- Improved boundary refinement

---

## 📚 References

- LIDC-IDRI dataset (Kaggle)
- Cicek et al., 3D U-Net
- Oktay et al., Attention U-Net

---

## 👨‍💻 Author

Ronit
```
