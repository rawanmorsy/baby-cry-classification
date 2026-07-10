<div align="center">

# 👶 Baby Cry Classification

### Deep Learning-based Infant Cry Classification using MobileNetV2

Classifying infant crying sounds into different categories using audio preprocessing, Mel Spectrograms, and Transfer Learning.

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange?style=for-the-badge&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras)
![Librosa](https://img.shields.io/badge/Librosa-AudioProcessing-green?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google-Colab-yellow?style=for-the-badge&logo=googlecolab)

</div>

---

# 📖 Overview

Infant crying is one of the primary ways babies communicate their needs. This project leverages Deep Learning to automatically classify baby crying sounds into different categories by converting audio signals into Mel Spectrogram images and training a MobileNetV2 model using Transfer Learning.

---

# ✨ Features

✅ Audio preprocessing

✅ Audio resampling (16 kHz)

✅ Mono audio conversion

✅ Noise reduction

✅ Audio length standardization (6 sec)

✅ Data augmentation & balancing

✅ Mel Spectrogram generation

✅ MobileNetV2 Transfer Learning

✅ Fine-tuning

✅ Focal Loss

✅ EarlyStopping

✅ ModelCheckpoint

✅ M Display Result in App
---

# 🧠 Model Pipeline

```text
Raw Audio
    │
    ▼
Convert to WAV
    │
    ▼
16 kHz + Mono
    │
    ▼
Noise Reduction
    │
    ▼
Trim / Pad (6 sec)
    │
    ▼
Data Augmentation
    │
    ▼
Mel Spectrogram
    │
    ▼
MobileNetV2
    │
    ▼
Fine-Tuning
    │
    ▼
Prediction
```

---

# 📂 Dataset

**Source**

- Baby Crying Sounds Dataset (Kaggle)

The dataset contains labeled infant crying audio recordings belonging to multiple cry categories.

---

# ⚙️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| Audio Processing | Librosa |
| Image Processing | OpenCV |
| Data Analysis | NumPy, Pandas |
| Visualization | Matplotlib |
| Development | Google Colab |

---

# 🔄 Data Preprocessing

The preprocessing pipeline performs the following steps:

- Convert audio to WAV format
- Resample to **16 kHz**
- Convert Stereo → Mono
- Remove corrupted files
- Remove very short clips
- Standardize audio length to **6 seconds**
- Apply Noise Reduction
- Perform Data Augmentation
- Balance the dataset
- Generate Mel Spectrograms
- Resize images to **224 × 224**

---

# 🏗 Model Architecture

**Base Model**

- MobileNetV2 (ImageNet Pretrained)

**Classification Head**

- GlobalAveragePooling2D
- Dense Layer
- Dropout
- Softmax Layer

**Training Strategy**

- Transfer Learning
- Fine-Tuning

**Loss Function**

- Focal Loss

**Optimizer**

- Adam

**Callbacks**

- EarlyStopping
- ModelCheckpoint

---

# 📊 Evaluation Metrics

The model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

# 📁 Project Structure

```text
Baby-Cry-Classification
│
├── Dataset
├── Preprocessing
├── Augmentation
├── Spectrograms
├── Models
├── Training Notebook.ipynb
├── Saved Models
├── requirements.txt
└── README.md
```

---

# 🚀 Future Work

- TensorFlow Lite deployment
- Flutter integration
- Real-time cry detection
- Transformer-based models
- Larger dataset


---

# 👩‍💻 Author

### Rawan Morsy

Flutter Developer • AI Enthusiast

---

⭐ If you found this project useful, don't forget to give it a Star!
