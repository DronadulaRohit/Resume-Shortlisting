# **Resume Shortlisting using ANN**

In today's competitive job market, recruiters often face the challenge of screening
hundreds of resumes in a short time. This project automates that process using an
**Artificial Neural Network (ANN)** that predicts whether a candidate should be
**shortlisted** based on their **academic performance** and **skill profile**.

The model is trained on a **synthetically generated dataset** of **1000 candidates**
and achieves **91% accuracy**, demonstrating that even a simple ANN can effectively
learn shortlisting patterns from structured candidate data.

---

## **Project Structure**

    ResumeShortlisting_ANN/
    │
    ├── data_generation.ipynb   # Synthetic dataset generation
    ├── main.ipynb              # Model training and evaluation
    ├── shortlisted.csv         # Generated dataset
    └── req.txt                 # Required libraries

---

## **Model Architecture**

- Input Layer — **7 features**
- Hidden Layer 1 — **16 neurons**, ReLU activation
- Hidden Layer 2 — **8 neurons**, ReLU activation
- Output Layer — **1 neuron**, Sigmoid activation
- Optimizer: **Adam**
- Loss: **Binary Crossentropy**
- EarlyStopping with **patience=10** and **restore_best_weights=True**

---

## **Features Used**

| **Feature** | **Description** |
|---|---|
| CGPA | Academic score (4.0 – 10.0) |
| Skills | Number of technical skills |
| Projects | Number of projects done |
| Certifications | Number of certifications |
| Internship | Internship experience (0 or 1) |
| Aptitude | Aptitude test score |
| Communication | Communication rating |

---

## **Results**

| **Metric** | **Score** |
|---|---|
| Accuracy | 91% |
| Precision (avg) | 0.92 |
| Recall (avg) | 0.91 |
| F1-Score (avg) | 0.91 |

---

## **Libraries Used**

- **TensorFlow / Keras**
- **Scikit-learn**
- **Pandas**
- **NumPy**
