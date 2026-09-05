# 🎓CAPSTONE PROJECT
# 🔐Cybersecurity Intrusion Detection Analysis

![PSPP](https://img.shields.io/badge/PSPP-Statistical%20Analysis-blue)
![Orange](https://img.shields.io/badge/Orange-Data%20Mining-orange)
![Logistic Regression](https://img.shields.io/badge/Model-Logistic%20Regression-green)
![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-red)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-purple)


A capstone project that uses **PSPP** and **Orange Data Mining** to analyze network traffic and predict cyber attacks using **Binary Logistic Regression**. The project combines statistical analysis with machine learning to identify the key factors associated with network intrusions.

---

## 📊Project Overview

This project investigates whether network session characteristics such as login behavior, IP reputation, encryption status, and session duration can be used to identify malicious activity.

Two analytical approaches were used:

- **PSPP** for statistical logistic regression analysis.
- **Orange Data Mining** for machine learning workflow and model evaluation.

The goal is to support data-driven intrusion detection by identifying the strongest predictors of cyber attacks.

---

## 🗂️Dataset

**Source:** Kaggle – Cybersecurity Intrusion Detection Dataset

[Uploading cybersecurity_intrusion_data.csv…]()

### Dataset Summary

| Item | Value |
|------|------:|
| Network Sessions | 9,537 |
| Features | 9 |
| Target Variable | attack_detected |
| Attack Sessions | 4,264 |
| Normal Sessions | 5,273 |

### Features

- Network Packet Size
- Protocol Type (TCP, UDP, ICMP)
- Login Attempts
- Failed Logins
- Session Duration
- Encryption Used
- IP Reputation Score
- Browser Type
- Unusual Time Access

**Target Variable**

- `attack_detected`
  - `1` = Attack
  - `0` = Normal Session

---

## 🛠️Tools & Technologies

| Tool | Purpose |
|------|---------|
| PSPP | Statistical Analysis |
| Orange Data Mining | Machine Learning Workflow |
| Logistic Regression | Classification Model |
| CSV Dataset | Data Source |

---

## 🤖Project Workflow

### ⚙️PSPP Workflow

1. Import CSV dataset.
2. Configure variable types.
3. Perform Binary Logistic Regression.
4. Evaluate model performance.
5. Interpret odds ratios and classification results.'

### 🔄PSPP Results

Regression Coefficients and P-Values

<img width="600" height="150" alt="image" src="https://github.com/user-attachments/assets/e3e8bdc6-8cc0-44f4-9ff4-0935494558c5" />

<img width="412" height="300" alt="image" src="https://github.com/user-attachments/assets/8b9b0632-502d-4b5e-9ad5-ac702c741879" />

<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/3c89c796-dc77-42c2-8dfe-ff5ce7b0f3b8" />

---

### ⚙️Orange Workflow

1. Import dataset.
2. Select features and target.
3. Preprocess the data.
4. Split data into **80% training** and **20% testing**.
5. Train a Logistic Regression model.
6. Evaluate performance using:
   - Confusion Matrix
   - ROC Curve
   - Performance Scores
   - Scatter Plot

<img width="1472" height="626" alt="ORANGE WORKFLOW" src="https://github.com/user-attachments/assets/fc7788b8-49a8-4fab-b56e-e81dacce6101" />


### 🔄Orange Results

Model Performance Summary
<img width="803" height="91" alt="image" src="https://github.com/user-attachments/assets/0ff51391-69bd-4ef5-ab24-f00907a0c53a" />

Confusion Matrix

<img width="470" height="247" alt="CONFUSION" src="https://github.com/user-attachments/assets/1e95e6fb-8316-4556-bdb9-36e11c31c858" />\

📈ROC Analysis — Attack Not Detected (Target Class 0)

<img width="955" height="662" alt="ROC CURVE - T0" src="https://github.com/user-attachments/assets/e06b389a-eeb0-4275-9d3f-0ede5c342eef" />

📈ROC Analysis — Attack Detected (Target Class 1)

<img width="955" height="645" alt="ROC CURVE - T1" src="https://github.com/user-attachments/assets/a07563a0-8002-47d5-a249-0326f7f0a5ce" />


---

## 📋Results - PSPP vs Orange
<img width="1530" height="618" alt="image" src="https://github.com/user-attachments/assets/2deb3031-184c-42cd-aec6-2e5b900c702b" />

---

### 👨‍💻Business Recommendations

- Prioritize IP reputation score
- Set automated failed-login alerts
- Deprioritize low-value features
- Deploy the Orange-trained model
- Use a tiered response system

---

## 👨‍💻Key Findings

- IP reputation score, failed logins, and login attempts are the strongest predictors. Network packet size and session       duration are not.
- Consistent findings across both tools add credibility to the results.
- Enables organizations to shift from reactive monitoring to proactive, automated detection.
- Orange outperforms PSPP higher accuracy (74.1% vs 72.9%) and recall (73.9% vs 65.6%).

---
## 👨‍💻Author

**Dhathri Narne**
