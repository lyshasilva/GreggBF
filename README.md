# HANDWRITTEN GREGG SHORTHAND BRIEF FORMS RECOGNITION USING CONVOLUTIONAL NEURAL NETWORKS
<!--
This is the public repository for my study on handwritten Gregg Shorthand brief forms recognition using Convolutional Neural Networks (CNNs). It contains the complete source code, confusion matrices, and access to the GreggBF Dataset used in the experiments.

The project evaluates and compares three adapted CNN models—**AlexNet**, **Inception-V3**, and **EfficientNetB0**—in recognizing 139 classes of handwritten Gregg Shorthand brief forms based on the Centennial Edition.-->

---

## 📚 GreggBF Dataset

**GreggBF** is a publicly available dataset of handwritten Gregg Shorthand brief forms, collected and annotated for machine learning and handwriting recognition research. The dataset includes **3,753** (`by_word.zip`) original handwritten samples expanded to **67,554** images (`augmented-split-by_word.zip`; currently not available due to storage limitation) through data augmentation across 139 classes

> ⚠️ **Note**: Due to size constraints, the dataset is not stored directly in this repository.

### 📥 Dataset Download

You can download the dataset from the following Dropbox link:

🔗 **[Download GreggBF Dataset](https://www.dropbox.com/scl/fo/76ciws7z0vtb3glgi9ixf/AIYCkYsANxKnzlj0r7xV2KE?rlkey=po4uefua5s70qj5bll6zqnfd9&st=m7eoel5r&dl=0)**

---
<!--
## 📁 Dataset Contents

The `Dataset` folder includes four zipped archives for different workflows:

1. ### `by_participant.zip` ❌ [Not available due to storage limitation]
   - **Original, augmentation-free samples**, grouped by **participant**  
   - 139 classes × 27 participants

2. ### `by_word.zip` ✅ **[Recommended]**
   - **Original, augmentation-free samples**, grouped by **class**
   - The starting dataset for the source code
   - 139 classes x 27 participants

3. ### `split-by_word.zip` **[Ongoing Upload]**
   - A **70/15/15** split (train/val/test) version of `by_word` 
   - For standardized evaluation
   - Can be duplicated using 'by_word.zip' by following the methodology and running the source code

4. ### `augmented-split-by_word.zip` ❌ [Not available due to storage limitation]
   - Augmented version of 'split-by-word'
   - Includes 17 augmentation variations per image  
   - Used in all model experiments
   - Can be reproduced using 'by_word.zip' or 'spit-by_word.zip' by following the methodology and running the source code
   - 📌 **Augmentations were applied *after* the dataset was split**, avoiding data leakage

---

## 🛠️ How to Use

1. Download `by_word.zip` from the link above.
2. Unzip the dataset.
3. Load it into your machine learning pipeline (e.g., TensorFlow, PyTorch).  
   - Each folder corresponds to one brief form class label.

---

## 📝 Data Collection and Validation

- Collected from **BSOA students** at **South Philippine Adventist College** with Gregg Shorthand exposure
- Approved by the program chairperson for research use
- **Not formally validated for symbol accuracy** — inconsistencies may exist
- For high-precision tasks, consider additional **data cleaning and validation**

---

## 📘 Project Scope

- Evaluates performance of **AlexNet**, **Inception-V3**, and **EfficientNetB0** on GreggBF
- Metrics used: **Accuracy**, **F1-score**, **ROC-AUC**, and **Confusion Matrix Analysis**
- Includes **source code**, **confusion matrix outputs**, and **thesis documentation**

-->
---

## 🔍 Keywords

Gregg Shorthand, Centennial Edition, brief forms, handwritten dataset, machine learning, deep learning, image classification, CNN, handwriting recognition, data augmentation

---
<!--
## 📚 Citation

If you use this dataset or any part of this repository, please cite:

> Silva, L. (2025). *Handwritten Gregg Shorthand Brief Forms Recognition Using Convolutional Neural Networks* (Unpublished undergraduate thesis). South Philippine Adventist College.

📌 This work is based on an undergraduate thesis currently in preparation/submission. The citation will be updated once officially archived or published.
-->
