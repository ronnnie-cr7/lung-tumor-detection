# 🫁 Lung Tumor Segmentation using 3D U-Net & Attention U-Net

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
- Evaluate performance using Dice Score and Hausdorff Distance

---

## 📂 Project Structure

```
lung-tumor-detection/
│
├── notebooks/
│   ├── M1_EDA_Analysis.ipynb
│   ├── M2_3D_UNet_Segmentation.ipynb
│   ├── M3_Data_Augmentation_Comparison.ipynb
│   └── M4_Attention_UNet_MC_Dropout.ipynb
│
├── results/
│   ├── figures/
│   │   ├── ct_slice_vs_mask.png
│   │   ├── ground_truth_vs_pred.png
│   │   ├── attention_unet.png
│   │   ├── 3dunet_vs_aug.png
│   │   └── sample0.png, sample1.png, sample2.png
│   └── stats/
│       └── statistics.png ... statistics6.png
│
├── .gitignore
└── README.md
```

---

## 🔍 Detailed Workflow

### 🔹 M1: Exploratory Data Analysis
- Visualized 3D CT scan slices
- Identified tumor vs non-tumor regions
- Analyzed class imbalance
- Preprocessed volumetric data (normalization, reshaping)

### 🔹 M2: Baseline 3D U-Net
- Implemented 3D U-Net with encoder–decoder + skip connections
- Input: 3D CT voxel volumes → Output: tumor segmentation masks
- Evaluation: Dice Score

### 🔹 M3: Data Augmentation
- Rotation, flipping, noise injection
- Improved generalization and reduced overfitting
- Significant Dice Score improvement over baseline

### 🔹 M4: Attention U-Net + MC Dropout
- Attention gates for focused tumor segmentation
- MC Dropout for per-voxel uncertainty estimation
- Outputs: Segmentation mask + Uncertainty map

---

## 📊 Data Split

| Split | Ratio | Purpose |
|-------|-------|---------|
| Train | 80% | Model training |
| Val | 20% | Evaluation |

> ⚠️ Due to limited dataset size, an 80/20 train/val split was used across all models to maximize training samples. A separate test set was not held out.

---

## 📈 Results Summary

| Model | Dice Score | Insight |
|-------|------------|---------|
| 3D U-Net (Baseline) | ~0.44 | Baseline performance |
| 3D U-Net + Augmentation | ~0.65 | Strong improvement |
| Attention U-Net + MC Dropout | ~0.68–0.70 | Best performance + uncertainty |

---

## 📊 Evaluation Metrics

- **Dice Score** — measures overlap between prediction and ground truth
- **Hausdorff Distance** — measures maximum boundary deviation
- **Uncertainty Map** — indicates model confidence per voxel

---

## 🫁 Dataset

- LIDC-IDRI dataset (Kaggle)
- 3D CT scans with voxel-level annotations
- Binary segmentation: tumor / non-tumor

---

## 🛠️ Tech Stack

- Python 3.x
- TensorFlow 2.x
- NumPy, OpenCV
- Matplotlib
- Google Colab

---

## 🚀 Future Improvements

- Dice + Focal loss for harder negatives
- HD95 metric integration
- Improved boundary refinement
- Gradio/Streamlit deployment

---

## 📚 References

- LIDC-IDRI dataset — Kaggle
- Çiçek et al., 3D U-Net (2016)
- Oktay et al., Attention U-Net (2018)

---

## 👨‍💻 Author

**Ronit**
