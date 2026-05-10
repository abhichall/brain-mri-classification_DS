# Brain MRI Tumor Classification Using Deep Learning

## Project Overview

This project's goal is to discover the effectiveness of convolutional neural networks (CNNs) and transfer learning models on classifying four classes of brain tumors from MRI scans. We use a custom baseline CNN against pre-trained transfer learning architectures such as MobileNetV2 and EfficientNetB0. We also did perform an augmentation experiment to analyze the impact of data augmentation on model generalization. This included augmentations such as flipping, rotating, dimming, etc to the data.

Our final paper -- attached to this repo as **\brainMRIClassificationPaper\_** - gathers all of the findings from this ML pipelining and summarizes it to focus on model comparison, preprocessing techniques, data augmentation, and overall performance in medical image classification.

---

# Dataset

Dataset Used:

- Brain MRI Tumor Dataset (Kaggle) -- [https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset?resource=download]

Tumor Classes:

- Glioma
- Meningioma
- Pituitary
- No Tumor

Dataset Structure:

```text
data/
├── Training/
├── Testing/
```

> Note: We included the `data/` folder within `.gitignore` because the dataset size exceeds GitHub storage limits. Please download it, and use it within its pre-format (testing/training)

---

# Models Implemented

1. Baseline CNN
2. MobileNetV2 Transfer Learning
3. EfficientNetB0 Transfer Learning
4. MobileNetV2 with Data Augmentation

---

# Final Results

| Model                      | Test Accuracy |
| -------------------------- | ------------- |
| Baseline CNN               | 91.70%        |
| MobileNetV2                | 87.36%        |
| EfficientNetB0             | 85.92%        |
| MobileNetV2 + Augmentation | 86.82%        |

### Key Finding

The custom CNN outperformed the transfer learning models on this MRI dataset. This suggests that a task-specific CNN may capture MRI features more effectively than pre-trained models with frozen feature extraction layers.

---

# Structure

```text
brain-mri-classification/
│
├── data/
├── notebooks/
├── figures/
├── models/
├── README.md
├── requirements.txt
└── final_report.pdf
```

---

# Notebooks

| Notebook                                | Purpose                                    |
| --------------------------------------- | ------------------------------------------ |
| 01_data_exploration.ipynb               | Dataset exploration and visualization      |
| 02_preprocessing_and_augmentation.ipynb | Preprocessing and augmentation pipeline    |
| 03_baseline_cnn.ipynb                   | Baseline CNN training                      |
| 04_mobilenet_transfer_learning.ipynb    | MobileNetV2 transfer learning              |
| 05_efficientnet_transfer_learning.ipynb | EfficientNetB0 transfer learning           |
| 06_model_evaluation.ipynb               | Confusion matrix and classification report |
| 07_augmentation_experiment.ipynb        | Augmentation experiment                    |
| 08_final_results_summary.ipynb          | Final model comparison and visualizations  |

---

# Installation

Install required packages:

```bash
pip install -r requirements.txt
```

---

# Running the Project

Run notebooks in order:

```text
01 → 08
```

---

# Paper

The final project paper is included as:

```text
final_report.pdf
```

---

# Authors

Abhi Challa, Sai Somisetty, Tejas Hariharan
