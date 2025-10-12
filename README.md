# Voice-Verification-Project
Voice Verification using Deep Learning — Learn speaker embeddings and verify voices live.

This project demonstrates a **Voice Verification System** using Deep Learning.  
The model was trained on **Kaggle** and later tested live with real voice recordings to verify speaker identity.

---

## 🎯 Objective

- Extract unique **speaker embeddings** for each individual  
- Verify whether two audio samples belong to the same speaker  
- Evaluate the system in real-time using microphone input  

---

## 📚 Notebook Contents

- Data exploration and preprocessing  
- Audio feature extraction (e.g., Mel-Spectrograms)  
- Model architecture (CNN / Siamese / Triplet network)  
- Training and evaluation  
- Metrics: ROC Curve, Equal Error Rate (EER), verification accuracy  
- Live testing: record your own voice and compare with stored samples  

---

## 🧰 Tools & Libraries

- **Python**  
- **Librosa** for audio preprocessing  
- **PyTorch** (or TensorFlow, depending on your code)  
- **Matplotlib / Seaborn** for visualization  
- **NumPy / Pandas**  

---

## ⚡ How to Run

1. Open the notebook on **Kaggle** (or run locally).  
2. Execute the cells step by step.  
3. For live testing: use the microphone recording cell to capture your voice.  
4. Compare two audio samples → the system outputs a similarity score.  

---

## 📊 Results

- Trained model achieved promising verification accuracy.  
- Successfully tested with **live voice recordings**.  
- The system was able to distinguish between same-speaker and different-speaker audio samples effectively.  
