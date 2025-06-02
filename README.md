# HANDWRITTEN GREGG SHORTHAND BRIEF FORMS RECOGNITION USING CONVOLUTIONAL NEURAL NETWORKS

This is the public repository for my study on handwritten Gregg Shorthand brief forms recognition using convolutional neural networks (CNNs). It contains the complete source code, the GreggBF Dataset, and confusion matrices generated from the experiments.

The project evaluates and compares three adapted CNN models—AlexNet, Inception-V3, and EfficientNetB0—for recognizing 139 classes of Gregg Shorthand brief forms using the GreggBF dataset.

## 📚 GreggBF Dataset

**GreggBF** is a publicly available dataset of **handwritten Gregg Shorthand brief forms (Centennial Edition)**, collected and annotated for use in machine learning and handwriting recognition research. This repository also includes supplementary materials from the accompanying undergraduate thesis on CNN-based recognition of these symbols.

📌 **Keywords**: Gregg Shorthand, Centennial Edition, brief forms, handwritten dataset, machine learning, deep learning, image classification, CNN, handwriting recognition, data augmentation

---

## 📦 Dataset Download

Because of file size limitations, the dataset is **not hosted directly in this repository**. You can download the full dataset from the following Dropbox link:

🔗 **[Download GreggBF Dataset](https://www.dropbox.com/scl/fo/76ciws7z0vtb3glgi9ixf/AIYCkYsANxKnzlj0r7xV2KE?rlkey=po4uefua5s70qj5bll6zqnfd9&st=m7eoel5r&dl=0)**

After downloading, extract the `.zip` file(s) and follow the usage instructions below.

---

## 📘 Overview

This repository provides the full dataset used in the study, including original and augmented samples across 139 shorthand brief form classes. These resources support reproducibility, further experimentation, and peer review of the results presented in the thesis.

---

## 📁 Contents

The `Dataset` folder contains four zipped archives, each structured to support different experimental workflows:

1. ### `by_participant.zip`
   - **Original handwritten samples**, grouped by participant.
   - 139 classes × 27 participants.

2. ### `by_word.zip`
   - Same data, grouped by class/word instead of participant.
   - 139 class folders.

3. ### `split-by_word.zip`
   - A 70/15/15 (train/val/test) split version of `by_word`.

4. ### `augmented-split-by_word.zip` ✅ **[Recommended]**
   - Augmented version of `split-by_word`, with 17 augmentation variations per image.
   - Structure: (1 original + 17 augmentations) × 139 classes.
   - **Used in the thesis experiments.**
   - 🛡️ **Note**: Augmentation was applied *after* splitting to prevent data leakage between sets.

---

## 📝 Data Source and Validation

- Collected from **BSOA students** at **South Philippine Adventist College** familiar with Gregg Shorthand.
- Approved by the program chairperson for academic use.
- **No formal validation** of handwriting correctness was conducted; inconsistencies may be present.
- Users are encouraged to perform additional **data cleaning or validation** for high-accuracy applications.

---

## 🛠️ How to Use

1. Download `augmented-split-by_word.zip` from the link above.
2. Unzip and load into your machine learning pipeline (e.g., TensorFlow, PyTorch).
3. Each class folder corresponds to one Gregg brief form label.

---

## 📝 Notes

- Class names follow Gregg Centennial brief forms.
- 27 participants contributed handwritten samples.
- Augmentations include geometric and visual noise variations.

---

## 📚 Citation

If you use this dataset or any part of this repository, please cite:

> Silva, L. (2025). *Handwritten Gregg Shorthand Brief Forms Recognition Using Convolutional Neural Networks* (Unpublished undergraduate thesis). South Philippine Adventist College.

📌 This work is based on an undergraduate thesis currently in preparation/submission. The citation will be updated once officially archived or published.
