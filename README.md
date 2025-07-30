# Credit Card Fraud Detection using Isolation Forest

This project applies the Isolation Forest algorithm to detect fraudulent transactions in a highly imbalanced credit card dataset. It demonstrates how anomaly detection can be used to uncover hidden outliers in real-world data.

---

## Dataset

**Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

* 284,807 transactions
* 492 labeled fraud cases (less than 0.2%)
* Features:

  * `V1` to `V28`: anonymized PCA components
  * `Time` and `Amount`: raw numerical features
  * `Class`: target label (0 = legitimate, 1 = fraud)

---

## Tools & Libraries

* **Python 3**
* `pandas`, `numpy`
* `matplotlib`, `seaborn`
* `scikit-learn`

---

## Steps Performed

### 1. Data Loading & Exploration

* Loaded CSV and checked for nulls
* Visualized class imbalance using bar plots

### 2. Preprocessing

* Standardized numerical features using `StandardScaler`
* Removed target column (`Class`) to treat this as an unsupervised problem

### 3. Modeling

* Applied Isolation Forest
* Contamination rate set equal to the observed fraud rate
* Converted predictions: -1 → 1 (fraud), 1 → 0 (not fraud)

### 4. Evaluation

* Compared predictions with actual `Class` labels
* Generated classification report and confusion matrix
* Visualized results with heatmaps

---

##  Results

* **Precision (fraud class):** \~0.29
* **Recall (fraud class):** \~0.83
* **F1-Score (fraud class):** \~0.43
* The model is effective at capturing a large portion of fraud cases (high recall), but with some false positives (lower precision)
* Confusion matrix and class distribution visuals helped interpret model performance
  
### Visuals

* Class distribution (fraud vs non-fraud)
* Confusion matrix

---

## What I Learned

* Addressing class imbalance in fraud detection
* Leveraging Isolation Forest for unsupervised anomaly detection
* Evaluating detection models using scikit-learn
* Structuring and documenting ML projects for GitHub

---

## Future Improvements

* Experiment with One-Class SVM or Autoencoders
* Hyperparameter tuning
* Deploy with Streamlit or Flask

---

## Credits

Crafted with curiosity, matcha, and a sprinkle of stress by **Gowthami** 
