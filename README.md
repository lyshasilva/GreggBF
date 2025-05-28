# GreggBF

**GreggBF** is the official repository for the supplementary materials of my undergraduate thesis on the recognition of handwritten **Gregg Shorthand Centennial Edition brief forms** using deep learning. This repository serves as a centralized archive for datasets and resources that were too extensive to be included directly in the appendices of the final manuscript.

## 📘 Overview

This repository provides the full dataset used in the study, including original and augmented samples across 139 shorthand brief form classes. These resources support reproducibility, further experimentation, and peer review of the results presented in the thesis.

## 📁 Contents

The `Dataset` folder contains four zipped archives, each organized to support different experimental workflows:

1. ### `by_participant.zip`
   - **Description**: Contains augmented samples grouped by participant.
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
   - **Use**: This is the **official dataset used in the thesis**. Recommended for reproduction and benchmarking.

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

> Silva, L. (2025). *HANDWRITTEN GREGG SHORTHAND BRIEF FORMS RECOGNITION USING CONVOLUTIONAL NEURAL NETWORKS*. Undergraduate Thesis, South Philippine Adventist College.

