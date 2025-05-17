# Machine-Learning

# 🗣️ Nepali ASR using Whisper & Hugging Face 🤖🇳🇵

This project fine-tunes OpenAI's Whisper model for **Automatic Speech Recognition (ASR)** in the **Nepali language**, using the [OpenSLR54 dataset](https://huggingface.co/datasets/iamTangsang/OpenSLR54-Nepali-ASR). It leverages Hugging Face 🤗 Transformers, Datasets, and Trainer API to build a complete ASR pipeline—from data preprocessing to training, evaluation (WER), and deployment.

---

## 📌 Features

- ✅ Fine-tuning of `openai/whisper-small` model for Nepali speech
- ✅ 100% dataset utilization
- ✅ Preprocessing and feature extraction using `WhisperProcessor`
- ✅ Evaluation with **WER** (Word Error Rate)
- ✅ TensorBoard support for training visualization
- ✅ Punctuation preserved in transcriptions
- ✅ Generates deployment-ready JSON files:
  - `preprocessor_config.json`
  - `tokenizer_config.json`
  - `vocab.json`
  - `special_tokens_map.json`
  - `config.json`
  - `added_tokens.json`

---

## 📂 Dataset

- 📚 Dataset: [`iamTangsang/OpenSLR54-Nepali-ASR`](https://huggingface.co/datasets/iamTangsang/OpenSLR54-Nepali-ASR)
- 🎧 Audio: `.wav` files with native Nepali speech
- ✍️ Labels: Clean transcriptions with punctuation

---

## 🛠️ Installation

```bash
pip install torch transformers datasets evaluate jiwer soundfile torchaudio accelerate librosa huggingface_hub tensorboard
