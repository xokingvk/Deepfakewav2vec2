# Deepfakewav2vec2
Audio Deepfake Detection

Fine-tuned wav2vec2 model for detecting AI-generated audio. Achieves 92.86% accuracy on the ASVspoof2019 benchmark.

Show Image

What it does

Upload any .wav, .mp3, or .flac file → get Real or Fake prediction with confidence score.

Performance

MetricScoreAccuracy92.86%Precision99.99%Recall92.05%F1-Score93.63%Equal Error Rate (EER)4.01%

Evaluated on ASVspoof2019 evaluation subset.

Model


Base: alefiury/wav2vec2-large-xlsr-53-gender-recognition-librispeech
Fine-tuned on: ASVspoof2019 (real vs spoofed audio)
Task: Binary classification — real / fake


Run it

Click the Colab badge above or open:
https://colab.research.google.com/drive/1vFBELq8RVLV495b54zoO42ZlS_1dbRhW?usp=sharing

Run all cells in order. Last cell launches the Streamlit app.

Files

FileDescriptionmodel.safetensorsFine-tuned model weights (1.3GB)config.jsonModel configpreprocessor_config.jsonAudio preprocessing configtraining_args.binTraining argumentsapp.pyStreamlit web app

Tech Stack


HuggingFace Transformers
PyTorch
librosa
Streamlit


License

Apache 2.0
