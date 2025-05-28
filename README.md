# GreggBF: Handwritten Gregg Shorthand Centennial Edition Brief Forms Dataset

**GreggBF** is a publicly available dataset of **handwritten Gregg Shorthand brief forms (Centennial Edition)**, collected and annotated for use in machine learning and handwriting recognition research. This repository also includes supplementary materials from the accompanying undergraduate thesis on CNN-based recognition of these symbols.

📌 **Keywords**: Gregg Shorthand, Centennial Edition, brief forms, handwritten dataset, machine learning, deep learning, image classification, CNN, handwriting recognition, data augmentation


## 📘 Overview

This repository provides the full dataset used in the study, including original and augmented samples across 139 shorthand brief form classes. These resources support reproducibility, further experimentation, and peer review of the results presented in the thesis.

## 📁 Contents

The `Dataset` folder contains four zipped archives, each organized to support different experimental workflows:

1. ### `by_participant.zip`
   - **Description**: Contains **original, augmentation-free handwritten samples** grouped by participant.
   - **Structure**: 139 classes × 27 participants.
   - Useful for participant-specific model analysis or inter-writer variability studies.

2. ### `by_word.zip`
   - **Description**: Contains the same data as `by_participant` but grouped by class/word rather than participant.
   - **Structure**: 139 class folders, each containing all samples.

3. ### `split-by_word.zip`
   - **Description**: A 70/15/15 split (train/val/test) version of `by_word`.
   - **Purpose**: Used for standard evaluation pipeline with consistent data partitioning.

4. ### `augmented-split-by_word.zip` ✅ **[Recommended]**
   - **Description**: An augmented version of `split-by_word`, with 17 augmentation variations applied per image.
   - **Structure**: `(1 original + 17 augmentations) × 139 classes`.
   - **Use**: This is the **official dataset used in the thesis**. Can serve as a baseline for evaluating models. Recommended for reproduction.
   - **🛡️ Note**: **The data was first split into training/validation/test sets before any augmentation was applied**. This ensures that augmented images derived from the same original are not duplicated across different splits, **preventing data leakage** during evaluation.

## 📝 Data Source and Validation

- The dataset was collected from **Bachelor of Science in Office Administration (BSOA)** students at **South Philippine Adventist College**, who had prior exposure to Gregg Shorthand writing.
- The **data collection process was reviewed and approved by the program chairperson**, ensuring its appropriateness for academic and research purposes.
- However, due to time constraints, the **actual handwritten outputs were not formally validated for symbol accuracy**. As such, there may be inconsistencies or miswritten forms within the dataset.
- If higher classification performance is required, **further data cleaning, outlier analysis, or handwriting validation** is highly recommended as future work.

## 📄 How to Use

- Download `augmented-split-by_word.zip` if you're replicating or extending the experiment from the paper.
- Unzip and load into your preferred machine learning pipeline (e.g., TensorFlow, PyTorch).
- Each class folder corresponds to one Gregg brief form label.

## 📝 Notes

- The class names follow the Gregg Centennial brief form labels.
- Handwritten samples were collected from 27 participants and manually labeled.
- Augmentations include geometric transformations and visual noise to simulate real-world variability.

## 📚 Citation

If you use this dataset or any part of this repository, please cite:

> Silva, L. (2025). *HANDWRITTEN GREGG SHORTHAND BRIEF FORMS RECOGNITION USING CONVOLUTIONAL NEURAL NETWORKS* (Unpublished undergraduate thesis). South Philippine Adventist College.

📌 This work is based on an undergraduate thesis currently in preparation/submission. The citation above will be updated once officially archived or published.

