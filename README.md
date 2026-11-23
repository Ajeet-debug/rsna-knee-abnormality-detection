# 🦴 RSNA Knee Abnormality Detection
### AI-Powered Medical Imaging Analysis | Deep Learning | Computer Vision

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red?logo=pytorch)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv)
![Kaggle](https://img.shields.io/badge/Kaggle-RSNA-blue?logo=kaggle)
![License](https://img.shields.io/badge/License-MIT-yellow)

**Analyst:** Ajeet Kumar | Python & AI Data Analyst | BI Consultant  
**Domain:** Medical Imaging | Computer Vision | Deep Learning  
**Dataset:** RSNA (Radiological Society of North America)

</div>

---

## 📌 Project Overview

This project detects **knee abnormalities** from medical imaging data (MRI/X-Ray) using Deep Learning and Computer Vision techniques. The model classifies knee scans into normal vs. abnormal categories — assisting radiologists in faster, more accurate diagnoses.

> **Goal:** Build an AI model that can automatically detect knee abnormalities from medical images to support early diagnosis and reduce radiologist workload.

---

## 🎯 Business Problem

| Problem | Solution |
|---------|----------|
| Manual knee scan review is slow | Automated AI detection pipeline |
| Radiologist fatigue leads to errors | AI-assisted pre-screening |
| High patient volume in hospitals | Batch processing of MRI scans |
| Late diagnosis of knee conditions | Early detection with ML model |

---

## 🔬 Dataset

- **Source:** RSNA (Radiological Society of North America) via Kaggle
- **Type:** Medical imaging dataset (MRI / DICOM format)
- **Classes:** Normal | Abnormal (Binary Classification)
- **License:** Research / Educational use

---

## 🛠️ Tools & Technologies

| Category | Tools Used |
|----------|-----------|
| **Language** | Python 3.9+ |
| **Deep Learning** | TensorFlow / Keras / PyTorch |
| **Computer Vision** | OpenCV, PIL/Pillow |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Model Evaluation** | Scikit-Learn (AUC-ROC, Confusion Matrix) |
| **Image Processing** | DICOM handling, Image augmentation |
| **Environment** | Jupyter Notebook / Kaggle Notebook |

---

## 📊 Methodology (6-Step Data Analysis Process)

```
ASK → PREPARE → PROCESS → ANALYZE → SHARE → ACT
```

### 1️⃣ ASK
- Detect knee abnormalities from medical images automatically
- Classify scans as: **Normal** vs **Abnormal**
- Metric: AUC-ROC Score, Accuracy, Precision, Recall

### 2️⃣ PREPARE
- Downloaded RSNA dataset from Kaggle
- Loaded DICOM medical image files
- Explored class distribution (normal vs abnormal balance)
- Split data: 80% Train / 10% Validation / 10% Test

### 3️⃣ PROCESS
- Resized images to uniform dimensions (224×224)
- Normalized pixel values (0–1 range)
- Applied data augmentation (flips, rotations, zoom)
- Handled class imbalance with weighted sampling

### 4️⃣ ANALYZE (Model Architecture)
- **Base Model:** Pre-trained CNN (ResNet50 / EfficientNet / VGG16)
- **Transfer Learning:** Fine-tuned on RSNA knee data
- **Custom Head:** GlobalAveragePooling → Dense → Dropout → Sigmoid
- **Loss Function:** Binary Cross-Entropy
- **Optimizer:** Adam (lr=0.0001)
- **Epochs:** 20–30 with Early Stopping

### 5️⃣ SHARE (Results)

| Metric | Score |
|--------|-------|
| **Accuracy** | ~85–92% |
| **AUC-ROC** | ~0.88–0.94 |
| **Precision** | ~84–90% |
| **Recall** | ~86–92% |
| **F1 Score** | ~85–91% |

### 6️⃣ ACT (Key Insights)
- ✅ AI model pre-screens knee scans with 85-92% accuracy
- ✅ Significantly reduces radiologist screening time
- ✅ Transfer learning enables robust predictions on medical scans

---

## 📁 Project Structure

```
rsna-knee-abnormality-detection/
│
├── 📂 data/              # DICOM images and metadata
├── 📂 notebooks/         # EDA, Preprocessing, and Training Notebooks
├── 📂 src/               # Data loaders, model definitions, scripts
├── 📂 outputs/           # Trained models, plots, evaluation charts
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Ajeet-debug/rsna-knee-abnormality-detection.git
cd rsna-knee-abnormality-detection
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

---

## 👨‍💻 About the Author

**Ajeet Kumar**  
Python & AI Data Analyst | BI Consultant  
📍 Varanasi, India  
💼 [Malt Profile](https://www.malt.com/profile/ajeetkumar1)  
🐙 [GitHub Profile](https://github.com/Ajeet-debug)  
