# brain-mri-classification

### Dataset Setup

The dataset itself is not included in this repository because of GitHub storage limitations and repository size best practices. Please download the dataset manually using the link above.

## Dataset

This project uses the **Brain Tumor MRI Dataset** created by Masoud Nickparvar on Kaggle. The dataset contains approximately 7,000+ MRI images categorized into four classes:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

The dataset is organized into separate training and testing folders and is used for multi-class image classification tasks in deep learning and computer vision research. :contentReference[oaicite:0]{index=0}

### Download Dataset

Download the dataset from Kaggle here:

[Brain Tumor MRI Dataset (Kaggle)](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset?utm_source=chatgpt.com)

### Dataset Setup

After downloading the dataset, extract it into the following directory structure:

```text
data/
├── training/
│   ├── glioma/
│   ├── meningioma/
│   ├── notumor/
│   └── pituitary/
│
└── testing/
    ├── glioma/
    ├── meningioma/
    ├── notumor/
    └── pituitary/

```
