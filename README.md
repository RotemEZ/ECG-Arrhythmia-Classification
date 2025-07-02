# ECG-Arrhythmia-Classification

# RhythmNet: Real-Time ECG Arrhythmia Classification with AI

This repository contains the full implementation and presentation of **RhythmNet**, a hybrid deep learning model designed for real-time arrhythmia detection from ECG signals. Developed as part of the *Advanced Machine Learning Workshop: From Research to Clinical Implementation*, this project combines clinical insight, signal processing, and AI modeling to support cardiac diagnosis in hospital environments.

---

## 🔍 Project Overview

Cardiac arrhythmias are a leading cause of sudden cardiac death and demand rapid, accurate diagnosis. Manual ECG interpretation in emergency settings is time-consuming and error-prone. **RhythmNet** addresses this gap by providing:

- Real-time arrhythmia classification with **<1 second** processing time  
- Support for **5 arrhythmia classes** (Normal, Supraventricular, Ventricular, Fusion, Unclassifiable)  
- High clinical performance: **98.54% accuracy**, **91.03% sensitivity**  
- Interpretable AI outputs with clinical decision support  
- Seamless integration with hospital monitoring systems  

---

## 📁 Repository Structure
```
.
├── notebooks/
│   └── RhythmNet_Model_Implementation.ipynb   # Complete model training & evaluation
├── presentation/
│   └── RhythmNet_Presentation_Final.pptx      # Project summary slides
├── README.md                                  # This file

```

---

## 📊 Dataset

We used the **MIT-BIH Arrhythmia Database**, publicly available on Kaggle.

📎 Download it from here:  
➡️ [Heartbeat Classification Dataset (Kaggle)](https://www.kaggle.com/datasets/shayanfazeli/heartbeat)

The dataset includes:
- ECG signals from 47 patients  
- 5 arrhythmia classification labels  
- 87,000+ heartbeat samples with expert annotations  

---

## 🧠 Model Summary

Our core model, **RhythmNet**, integrates:

- 1D Convolutional Neural Networks (CNNs) for local ECG pattern recognition  
- Attention and Transformer layers for modeling global temporal dependencies  
- SMOTE oversampling to address severe class imbalance  
- Multi-domain feature engineering: statistical, morphological, temporal, spectral, entropy, and wavelet features  

We benchmarked RhythmNet against:
- ViT-1D Transformer  
- XGBoost with handcrafted features  
- Traditional machine learning baselines  

---

## 📈 Results

| Model               | Accuracy | F1-Score | Sensitivity | Specificity |
|---------------------|----------|----------|-------------|-------------|
| RhythmNet (Hybrid)  | 98.54%   | 92.33%   | 91.03%      | 98.89%      |
| ViT-1D Transformer  | 98.28%   | 91.47%   | 89.99%      | 98.70%      |
| XGBoost + SMOTE     | 98.29%   | 90.66%   | 90.54%      | 98.70%      |

✅ *RhythmNet achieves the best trade-off between accuracy, sensitivity, and real-time speed.*

---

## 🚀 Future Work

- Large-scale prospective validation in clinical settings  
- Integration with additional vital signs (e.g., SpO2, BP)  
- Cloud and edge deployment for scalable, low-latency inference  
- Federated learning for privacy-preserving cross-hospital collaboration  

---

## 👥 Team

**Project Group 25 – Data Science in Industry**  
Rotem Even Zur • Nevo Levi • Guy Kalati  

---

## 📬 Contact

For questions or collaboration, feel free to open an issue or contact us directly.

---

> *This project was developed at Ben-Gurion University as part of the "Advanced Machine Learning Workshop".*
