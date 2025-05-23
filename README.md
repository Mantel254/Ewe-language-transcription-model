# 🧠 Fine-Tuning Audio Transcription with CNN + CTC

This project demonstrates fine-tuning a speech-to-text model using Ewe-language audio data. It covers data preprocessing, spectrogram augmentation, training a convolutional neural network (CNN), and evaluating transcription accuracy using Character Error Rate (CER).

---

## 📁 Overview

- Load and clean transcription data from an Excel file
- Process raw audio into Mel Spectrograms with augmentation
- Train a custom CNN model using **CTC Loss**
- Evaluate predictions using **greedy decoding** and `jiwer` CER

---

## 🔧 Setup

### Install Dependencies
Run this in a Google Colab cell or local environment:

```bash
pip install torchaudio numpy gensim jiwer
sudo apt-get install ffmpeg
```
# Data
📊 **Dataset Source**: [SciDB - Ewe Speech Dataset](https://www.scidb.cn/en/detail?dataSetId=bbd6baee3acf43bbbc4fe25e21077c8a)

data[https://www.scidb.cn/en/detail?dataSetId=bbd6baee3acf43bbbc4fe25e21077c8a]
```
Ewe/
├── selected transcribed audios/
│   ├── audios/
│   │   ├── *.wav
│   └── selected transcribed audios.xlsx

