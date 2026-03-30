## 📌 Overview

Postoperative pain following endodontic treatment remains a frequent and clinically relevant outcome, even when procedures are performed within accepted technical standards. Its occurrence is inherently multifactorial and often unpredictable, resulting from complex interactions between patient-related, tooth-related, and treatment-related factors.

This variability limits the clinician’s ability to anticipate pain and implement preventive strategies, which may negatively impact patient experience, treatment perception, and clinical decision-making. Traditional approaches rely on isolated factors and linear interpretations, which may not adequately capture the complexity of this phenomenon.

In this context, machine learning (ML) offers a data-driven approach capable of modelling non-linear relationships and integrating multiple clinical variables simultaneously, enabling more accurate and individualized risk prediction.

---

## ⚙️ Methodology

### Study Design

A prospective dataset was constructed using clinical and demographic data collected from patients undergoing endodontic treatment of teeth with pulp necrosis.

### Target Variable

Postoperative pain was assessed using a visual analogue scale (VAS) and subsequently dichotomized into:

* Presence of pain
* Absence of pain

Predictions were performed at:

* 24 hours
* 48 hours
* 72 hours

---

### Input Features

The models were trained using routinely collected clinical variables, including:

* Demographic factors (e.g., age, sex)
* Treatment-related variables
* Procedural characteristics

These variables were selected based on their clinical relevance and availability in real-world settings.

---

### Machine Learning Models

A total of **eight supervised machine learning algorithms** were implemented, representing different modelling approaches, including:

* Linear models
* Tree-based models
* Ensemble methods
* Distance-based algorithms
* Neural networks

---

### Model Development Pipeline

The modelling workflow followed standard machine learning practices:

1. **Data Splitting**

   * Training set: 80%
   * Test set: 20%

2. **Hyperparameter Optimisation**

   * Grid Search

3. **Model Validation**

   * 5-fold cross-validation

4. **Performance Evaluation**

   * Accuracy
   * Precision
   * Recall
   * F1-score
   * Area Under the ROC Curve (AUC)

5. **Uncertainty Estimation**

   * 95% Confidence Intervals obtained via bootstrapping

---

### Clinical Application Perspective

The proposed models are designed to be integrated into clinical workflows through digital interfaces, enabling real-time risk estimation based on routinely collected patient data. This approach supports clinical decision-making by providing individualized predictions without increasing procedural complexity.

---
