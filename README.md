# Smartphone Privacy Risk Classifier  
### *A Machine Learning Study of Android App Permissions & Privacy Risk*

**Project Website:** [To be updated]

---

# Overview

This project investigates the privacy risk of **29,999 Android apps** by analyzing their system permissions, metadata, and user engagement patterns.  
Using Exploratory Data Analysis (EDA) and Machine Learning, the project identifies:

- which app behaviors indicate higher privacy risk,  
- how dangerous permissions correlate with user trust,  
- which app categories request the most sensitive data, and  
- how effectively machine learning can predict privacy risk.

The goal is to demonstrate **high-quality analytical and research skills**, suitable for **Research Assistant roles** and advanced academic projects.

---

# Objectives

1. Clean and preprocess a high-dimensional Android permissions dataset  
2. Conduct extensive EDA on permission patterns and app characteristics  
3. Test seven research-backed privacy hypotheses  
4. Build a machine learning model to classify apps into risk levels  
5. Interpret the model using feature importance and category patterns  
6. Publish results through a polished, interactive project website  

---

# Dataset Description

**Source:** Android app metadata & permissions dataset from Kaggle  

### Key Fields
- **App metadata:** name, package, description, category, rating, price  
- **User engagement:** number of ratings  
- **Permissions (170+ columns):** dangerous vs safe permissions  
- **Permission aggregates:**  
  - *Dangerous permissions count*  
  - *Safe permissions count*  
- **Class:** Low / Medium / High risk  

After processing:
- **184 total columns**  
- Mostly binary permission indicators  
- Significant sparsity → ideal for tree-based models  

---

# Tech Stack

### Programming & Analysis  
- Python (Pandas, NumPy)  
- Matplotlib, Seaborn  

### Machine Learning  
- Scikit-learn (Random Forest Classifier)  
- Feature Importance Analysis  

### Web Deployment  
- HTML, CSS, JavaScript  
- GitHub Pages (static website)  

---

# Research Hypotheses

This project evaluates **7 privacy hypotheses** derived from app-security literature and user-trust studies.

### **H1 — Dangerous permissions correlate with lower app ratings.**  
Users distrust apps requesting sensitive access.

### **H2 — Apps with higher dangerous-permission count are more likely to be high-risk.**  
Core premise for risk classification.

### **H3 — App categories differ significantly in privacy risk.**  
Communication, Tools, and Productivity apps request the most sensitive permissions.

### **H4 — Price and privacy-risk interact.**  
Free apps depend more heavily on personal data and request more permissions.

### **H5 — Popularity (ratings count) is negatively correlated with dangerous permissions.**  
Risky apps receive lower adoption.

### **H6 — Specific permissions strongly predict privacy risk.**  
SMS, phone identity, location, and storage modification are key signals.

### **H7 — Machine learning can classify privacy risk with >80% accuracy.**  
Shown through model evaluation and confusion matrix.

All hypotheses are tested and visualized in the **Hypotheses** section of the website.

---

# Exploratory Data Analysis

Major analyses include:

- Distribution of dangerous permissions  
- Category-wise permission usage  
- Correlation heatmap of numeric variables  
- Rating vs permission patterns  
- Popularity vs risk indicators  
- Feature distributions and outliers  

All corresponding visualizations are available under **EDA** on the website.

---

# Machine Learning Model

### **Model Used:** Random Forest Classifier  
Chosen due to:
- strong performance on sparse, high-dimensional data  
- robustness to multicollinearity  
- ability to capture non-linear patterns  

### **Results**
- **Accuracy:** ~80%  
- Strong recall for high-risk apps  
- Distinct separation between low-risk and high-risk patterns  

### Key Predictors
- Number of ratings  
- Category  
- Price  
- Dangerous permissions count  
- Specific sensitive permissions (GPS, SMS, phone identity, storage control)

Feature importance plots and confusion matrix are shown in the **Hypotheses** and **EDA** sections.

---

# Key Insights

### 1. **High-risk apps display clear permission-based signatures.**  
Dangerous-permission-heavy apps form strong, detectable clusters.

### 2. **Category heavily influences risk.**  
Communication and Tools apps are consistently more privacy-demanding.

### 3. **Free apps request more sensitive permissions.**  
Suggests monetization through ads or user data.

### 4. **Popularity predicts trustworthiness.**  
Low-download apps tend to request more invasive permissions.

### 5. **Machine learning is effective for privacy screening.**  
The model provides scalable, automated risk detection.

---

# Website Structure

The website contains three polished sections:

- **Home:** Project overview  
- **EDA:** All analytical plots  
- **Hypotheses:** Detailed evidence for all 7 tested hypotheses  

Fully built using HTML/CSS/JS and deployed via GitHub Pages.

---

# Future Work

Planned extensions:

- Train XGBoost / LightGBM for performance comparison  
- Add SHAP value explanations for deeper interpretability  
- Build a real-time Risk Prediction web app  
- Cluster apps by permission patterns (unsupervised learning)  
- Add category-level privacy summaries  
- Deploy model as an API endpoint  

---

# Acknowledgments

Dataset sourced from the **Android permissions dataset on Kaggle**.  
All analysis, modeling, and website development by **Arushi Arunkumar**.

---

# Contact

For collaborations or research inquiries:  
📧 **arushiarunkumar@gmail.com**  
🔗 **LinkedIn:** https://www.linkedin.com/in/arushi-arunkumar/  
🐙 **GitHub:** https://github.com/ArushiArunkumar
