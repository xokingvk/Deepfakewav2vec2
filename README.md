# Deepfakewav2vec2
---
 
# Audio Deepfake Detection
 
Fine-tuned wav2vec2 model for detecting AI-generated audio. Achieves 92.86% accuracy on the ASVspoof2019 benchmark.
 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vFBELq8RVLV495b54zoO42ZlS_1dbRhW?usp=sharing)
 
## What it does
 
Upload any `.wav`, `.mp3`, or `.flac` file → get Real or Fake prediction with confidence score.
 
## Performance
 
| Metric | Score |
|---|---|
| Accuracy | 92.86% |
| Precision | 99.99% |
| Recall | 92.05% |
| F1-Score | 93.63% |
| Equal Error Rate (EER) | 4.01% |
 
Evaluated on [ASVspoof2019](https://www.kaggle.com/datasets/awsaf49/asvpoof-2019-dataset) evaluation subset.
 
## Model
 
- **Base:** `alefiury/wav2vec2-large-xlsr-53-gender-recognition-librispeech`
- **Fine-tuned on:** ASVspoof2019 (real vs spoofed audio)
- **Task:** Binary classification — `real` / `fake`
## Run it
 
Click the Colab badge above or open:
https://colab.research.google.com/drive/1vFBELq8RVLV495b54zoO42ZlS_1dbRhW?usp=sharing
 
Run all cells in order. Last cell launches the Streamlit app.
 
## Files
 
| File | Description |
|---|---|
| `model.safetensors` | Fine-tuned model weights (1.3GB) |
| `config.json` | Model config |
| `preprocessor_config.json` | Audio preprocessing config |
| `training_args.bin` | Training arguments |
| `app.py` | Streamlit web app |
 
## Tech Stack
 
- HuggingFace Transformers
- PyTorch
- librosa
- Streamlit
## License
 
Apache 2.0
 
---
 
