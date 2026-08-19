# Vietnamese Banknote Recognition (CNN)

This project uses a custom **Convolutional Neural Network (CNN)** built from scratch using `Keras` and `TensorFlow` to classify 11 circulating denominations of Vietnamese currency.

---

## Project Overview

* **Objective:** Automatically recognize and classify 11 Vietnamese banknote denominations (both polymer and paper notes).
* **Model:** Custom CNN model optimized to extract color patterns and visual features of banknotes.
* **Training:** Trained over 50 epochs using data augmentation techniques.

---

## Pre-trained Model

Due to GitHub's file size limits for model weight files (`.h5`), the trained model is hosted on Google Drive:

* **Banknote Recognition Model:** 👉 [Download `mo_hinh_nhan_dien_tien_50_epochs2.h5`](https://drive.google.com/file/d/1t9eL14Qoz3lDkMTycntEU6tC-pBlIaFX/view?usp=sharing)

---

## How to Use

Download the `.h5` model file and load it using `tensorflow.keras`:

```python
from tensorflow.keras.models import load_model

# Load the pre-trained model
model = load_model('mo_hinh_nhan_dien_tien_50_epochs2.h5')

print("Banknote recognition model ready for inference!")
