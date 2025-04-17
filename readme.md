# 🎙️ Deepfake Audio Detection using CNN & Spectrograms

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Torch](https://img.shields.io/badge/PyTorch-Used-red?logo=pytorch)
![Librosa](https://img.shields.io/badge/Librosa-Audio-green?logo=librosa)
![Status](https://img.shields.io/badge/Status-In_Progress-yellow)

---

## 📌 Overview

This project focuses on detecting **deepfake audio** using a **Convolutional Neural Network (CNN)** trained on **mel spectrograms** extracted from `.wav` files. With the rise of synthetic voices and AI-generated speech, this model helps identify fake audio recordings with high accuracy.

---

## 🧠 Objective

🎯 Build a deep learning model to:
- Differentiate between **real** and **fake** audio samples
- Use **mel spectrograms** for feature extraction
- Apply **CNN** to classify audio effectively
- Evaluate performance on separate train, validation, and test sets

---

## 🗂️ Dataset Structure
/for-rerecorded/ ├── training/ │ ├── real/ │ └── fake/ ├── validation/ │ ├── real/ │ └── fake/ └── testing/ ├── real/ └── fake/

- Format: `.wav`
- Labels: **real (0)**, **fake (1)**

---

## 🔧 Tech Stack

| Tool        | Purpose                                |
|-------------|----------------------------------------|
| **Python**  | Core programming language              |
| **Google Colab** | Development and training environment |
| **Librosa** | Basic audio loading & inspection       |
| **Torchaudio** | Advanced waveform loading, mel spectrograms |
| **PyTorch** | Deep learning framework (CNN model)    |
| **Matplotlib/Seaborn** | Data visualization          |

---

## 🧪 Key Features

- 🔉 Audio loading and processing via `torchaudio`
- 🎛️ Mel spectrogram transformation & dB scaling
- 🧱 Custom PyTorch Dataset class
- 🧠 CNN classifier with softmax output
- 📈 Evaluation with accuracy, F1-score, confusion matrix
- 🔍 Inference function for single-file prediction

---

## 🧬 Model Pipeline

.wav Audio ➡ Torchaudio Preprocessing ➡ Mel Spectrogram ➡ CNN ➡ Real/Fake

---

## 🚀 Future Improvements

- Add data augmentation (noise, pitch shift, etc.)
- Test on cross-dataset generalization
- Try transformers or spectrogram-based vision models

---

## 🤝 Contributing

Feel free to fork, open issues, or submit PRs!  
For suggestions, reach out via GitHub or email.

---

## 📁 How to Run

1. Upload dataset to Google Drive
2. Open `Deepfake_Audio_Detection.ipynb` in Google Colab
3. Run all cells to:
   - Load and preprocess data
   - Train the CNN
   - Evaluate model
   - Test on new audio samples
