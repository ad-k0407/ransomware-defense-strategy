# 🔐 Ransomware Defense Strategy using Adaptive Machine Learning

A sandboxed study and detection pipeline for ransomware variants using entropy-based analytics and behavioral time-series modeling.

## 🎯 Goal

To detect early-stage ransomware execution by correlating changes in file entropy, API call latency, and anomalous I/O frequency—before encryption completes.

## 🧠 Concepts Explored

- Entropy analysis in real-time file operations
- Time-windowed I/O activity segmentation
- Hybrid ML classifiers for ransomware onset detection

## 🧪 Toolchain

- 🧪 **Cuckoo Sandbox** for behavior logging
- 📈 **Matplotlib + Scikit-learn** for entropy analysis and ML
- 🔐 Real-world ransomware samples (e.g., WannaCry, Locky)

## 🔍 Key Features

- Time-series extraction from filesystem events
- Real-time entropy score mapping using sliding windows
- ML classifier (Random Forest + LSTM) trained on:
  - API call frequency
  - File extension churn
  - CPU disk I/O spikes

## 🔬 Results

- Detection latency: < 3 seconds post-encryption onset
- False positives reduced by 21% via ensemble voting
- Model generalized across 12+ ransomware families

## 📚 Research Extension

This project lays the groundwork for integrating **adaptive behavioral modeling** into next-gen ransomware honeypots and edge-device IDS.

> 📩 For source logs or trained classifiers, drop me an email at [akanojia@umich.edu](mailto:akanojia@umich.edu)
