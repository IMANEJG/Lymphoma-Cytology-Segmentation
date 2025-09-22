# 🧫 Lymphoma Cytology Segmentation – Benchmark of Deep Learning Models

This repository contains the code and notebooks developed for my scientific study  
**“Deep Learning for Lymphoma Diagnosis: A Cytology-Based Study Using Digitized Lymph Node Imprints.”**

---

## 📝 Project Overview

Accurate and reproducible analysis of cytology slides of lymph node imprints is essential for lymphoma diagnosis.  
Manual delineation of cells and regions is time-consuming and subject to observer variability.

This project investigates whether **deep learning architectures** can automatically segment and classify relevant regions on digitized cytology slides.  
Three state-of-the-art architectures were implemented and compared:

- **U-Net**
- **U-Net++**
- **DeepLabV3+**

Each model was trained and evaluated on the same dataset, with both **quantitative metrics** and **qualitative evaluation** by expert cytopathologists.

---

## 🗂️ Dataset and Annotation

- **Origin:** 148 cytology slides of lymph node imprints collected at **CHU Caen, France (2021–2023)**.  
- **Annotation tool:** **QuPath** was used by a junior pathologist to annotate the regions, then validated by an experienced cytopathologist.  
- **Confidentiality:** the raw images cannot be distributed; only the code is provided in this repository.

---

## 🧪 Benchmark of Deep Learning Models

For each model, the notebooks include:

- Data loading and preprocessing steps.
- Model architecture definition.
- Training and validation loops.
- Quantitative metrics such as Accuracy, Sensitivity, Specificity, Precision, F1-score, Dice, IoU, Jaccard, AUC, Cohen’s Kappa, Hausdorff Distance, Mean Surface Distance, etc.
- **Qualitative evaluation**: expert cytopathologists graded the predictions (“Excellent”, “Very good”, etc.) to assess clinical usability.

This dual evaluation ensures both statistical performance and clinical relevance.

---

## 📂 Repository Structure

```
Lymphoma-Cytology-Segmentation/
├── notebooks/ # All notebooks go here
│ ├── 3class_DeepLabV3+.ipynb # DeepLabV3+ implementation
│ ├── 3class_U-Net.ipynb # U-Net implementation
│ └── 3class_U-Net++.ipynb # U-Net++ implementation
├── data/ # (empty) explain data location and confidentiality
│ └── README.md
├── report/ # Paper or PDF report related to this study
│ └── Article.pdf
├── requirements.txt # Python dependencies
└── README.md # This file
```

---

## ⚙️ Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/IMANEJG/Lymphoma-Cytology-Segmentation.git
cd Lymphoma-Cytology-Segmentation
pip install -r requirements.txt
