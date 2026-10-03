# Brain Tumor MRI Classification

Binary image classification of **brain MRI scans — tumor vs. no tumor** — using a neural network built with **PyTorch**.

> **Author / Autor:** Hugo Benjumea Martínez · [github.com/Hben8](https://github.com/Hben8)

---

## 🇬🇧 English

### Overview
Deep‑learning project that classifies brain MRI images as **tumor** or **no tumor**. The pipeline:
1. Loads the images with `torchvision.datasets.ImageFolder`.
2. Preprocesses them: **resize to 64×64**, **grayscale**, **to tensor**, **normalization**.
3. Trains a fully‑connected neural network (`BCELoss`, `Adam` optimizer).
4. Evaluates accuracy on a held‑out test set.

### Dataset (not included)
The **Brain Tumor MRI** dataset (~7,000 images) is **excluded from the repository** because of its size. Download it (e.g. the *Brain Tumor MRI Dataset* on [Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)) and arrange it as:
```
Training/
  0/   # images WITHOUT tumor
  1/   # images WITH tumor
```

### Tech stack
Python · PyTorch · torchvision · Pillow · NumPy · Matplotlib

### How to run
```bash
pip install torch torchvision pillow numpy matplotlib
jupyter notebook brain_tumor_mri_classification.ipynb
```

### Possible improvements
Replacing the fully‑connected network with a **Convolutional Neural Network (CNN)** and adding data augmentation would be the natural next step to boost accuracy.

---

## 🇪🇸 Español

### Descripción
Proyecto de *deep learning* que clasifica imágenes de resonancia magnética (MRI) cerebral como **con tumor** o **sin tumor**. El flujo:
1. Carga las imágenes con `torchvision.datasets.ImageFolder`.
2. Las preprocesa: **redimensionado a 64×64**, **escala de grises**, **tensor** y **normalización**.
3. Entrena una red neuronal totalmente conectada (`BCELoss`, optimizador `Adam`).
4. Evalúa la *accuracy* sobre un conjunto de test.

### Dataset (no incluido)
El dataset **Brain Tumor MRI** (~7.000 imágenes) está **excluido del repositorio** por su tamaño. Descárgalo (p. ej. el *Brain Tumor MRI Dataset* de [Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)) y organízalo así:
```
Training/
  0/   # imágenes SIN tumor
  1/   # imágenes CON tumor
```

### Tecnologías
Python · PyTorch · torchvision · Pillow · NumPy · Matplotlib

### Cómo ejecutarlo
```bash
pip install torch torchvision pillow numpy matplotlib
jupyter notebook brain_tumor_mri_classification.ipynb
```

### Mejoras posibles
Sustituir la red totalmente conectada por una **red neuronal convolucional (CNN)** y añadir *data augmentation* sería el siguiente paso natural para mejorar la precisión.
