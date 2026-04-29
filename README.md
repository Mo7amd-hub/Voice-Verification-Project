# Overview

This project implements a voice verification system that can identify speakers by analyzing their voice characteristics. It uses a deep learning approach with a Siamese network architecture trained on triplet loss to create speaker embeddings that can differentiate between different speakers.

**Key Features:**
- Speaker identification from voice recordings
- Live speaker recognition using microphone input
- Uses MFCC for feature extraction
- Siamese Network with Triplet Loss for high-quality embeddings
- Fast and lightweight inference

## Project Structure

```
Voice-Verification-Project/
├── Model/
│   └── Voice_verification_model.h5       # Pre-trained Siamese model
├── voices/                               # Speaker voice samples
│   ├── aew/                             # Speaker 1 samples
│   └── silence/                         # Silence/background samples
├── notebook/
│   └── voice-verification.ipynb         # Full training pipeline
├── record.py                            # Script to record new voice samples
├── live_test.py                         # Script for live speaker recognition
└── README.md                            # This file
```

### 🛠 Tech Stack

- Python
- TensorFlow/Keras
- librosa
- numpy
- sounddevice
- scipy

### Setup

1. Install dependencies:
```bash
pip install tensorflow keras librosa numpy sounddevice soundfile scipy scikit-learn tqdm torch torchaudio pandas
```

2. Clone the project and navigate to the directory.

## Usage

Use `record.py` to record new voice samples from your microphone:

```bash
python record.py
```
This will record 10 audio clips of 3 seconds each for a speaker named "NewPerson" by default.

### Live Speaker Recognition

Run `live_test.py` to start real-time speaker recognition:

```bash
python live_test.py
```

## 🧠 How It Works

- Convert audio → MFCC features
- Pass features into embedding model
- Generate vector representation (embedding)
- Compare embeddings using cosine similarity
- Predict closest speaker

## Future Enhancements

- [ ] Add confidence threshold
- [ ] speaker enrollment for new users
- [ ] Multi-speaker detection
- [ ] Optimize model for mobile/edge deployment
- [ ] Implement voice liveness detection

## Author
Mohammed Mostafa

## 📎 Notes
For full training details and implementation, check the notebook inside the project.
You can also explore it on Kaggle: [(https://www.kaggle.com/code/mo7amed05/voice-verification-model)]
