# 🌿 Leaf Disease Detection

> A complete deep learning project for detecting diseases in plant leaves using Convolutional Neural Networks (CNN).  
> Includes data preprocessing, training, evaluation, and inference scripts for easy reproducibility.

---

## 📘 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Installation](#installation)
- [Usage](#usage)
  - [Prepare Data](#prepare-data)
  - [Training](#training)
  - [Evaluation](#evaluation)
  - [Prediction](#prediction)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🧩 Overview

This repository implements a **Leaf Disease Detection** system using CNNs to classify plant leaf images into healthy or diseased categories.  
The goal is to assist farmers and researchers in **early disease detection** to improve crop yield and reduce manual inspection efforts.

The project can be easily adapted for other plant species or datasets by changing the training data.

---

## 🚀 Features

✅ Image preprocessing and augmentation  
✅ Configurable CNN model  
✅ Model training with checkpoints  
✅ Evaluation metrics and confusion matrix  
✅ Inference for single image prediction  
✅ Modular, beginner-friendly structure  

---

## 🌱 Dataset

You can use the [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease) or your own collection of leaf images.

Expected folder layout:

data/
├── train/
│ ├── healthy/
│ └── diseased/
└── test/
├── healthy/
└── diseased/


Each class should have its own subfolder containing respective images.

---

## 📂 Project Structure

Leaf-Disease-Detection/
├── Target/
├── Final_Leaf_Disease_Detection (1).ipynb
├── plant_village.csv
├── a.jpg
├── README.md




---

## ⚙️ Getting Started

### Requirements

- Python 3.8+
- Libraries:
  - `torch` or `tensorflow` (depending on framework)
  - `numpy`, `matplotlib`, `pandas`, `scikit-learn`
  - `opencv-python` or `Pillow`

### Installation

```bash
# Clone the repository
git clone https://github.com/ShreyashButley/Leaf-Disease-Detection.git
cd Leaf-Disease-Detection

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows

# Install dependencies
pip install -r requirements.txt
```
Training
python src/train.py --data_dir data --epochs 30 --batch_size 32 --lr 0.0001 --save_dir checkpoints/

Evaluation
python src/evaluate.py --data_dir data --model_path checkpoints/best_model.pth

Prediction
python src/predict.py --image path/to/image.jpg --model_path checkpoints/best_model.pth


Example Output:

Predicted Class: Tomato___Bacterial_spot
Confidence: 98.7%

# output 
<img width="533" alt="image" src="https://user-images.githubusercontent.com/95575935/224718200-66f9d439-f5ee-430e-9963-71835186f073.png">


📧 Contact

Author: Shreyash Butley
GitHub: @ShreyashButley

