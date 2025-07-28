🕵️‍♀️ Credit Card Fraud Detection using Isolation Forest

This project uses the Isolation Forest algorithm to detect fraudulent transactions in a highly imbalanced credit card dataset. It’s a classic case of anomaly detection — where the goal is to find the sneaky, suspicious outliers hiding in a sea of normal data.

⸻

📂 Dataset
	•	Source: Kaggle -[Credit Card Fraud Detection] (https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)`

	•	Contains 284,807 transactions with 492 frauds
	•	Features:
‣ 28 anonymized numerical features (PCA components)
‣ Time and Amount
‣ Class (0 = legit, 1 = fraud)

⸻

🛠️ Tools & Libraries
	•	Python 🐍
	•	pandas, numpy
	•	matplotlib, seaborn
	•	scikit-learn (for Isolation Forest)

⸻

🧠 Steps Performed
	1.	Data Loading & Exploration
	•	Checked for missing values
	•	Visualized class imbalance
	2.	Preprocessing
	•	Standardized the numerical features
	•	Removed the target column (Class) for unsupervised learning
	3.	Modeling
	•	Applied Isolation Forest with a contamination rate matching the actual fraud rate
	•	Labeled predictions as anomaly or not
	4.	Evaluation
	•	Compared model output to actual Class labels
	•	Calculated precision, recall, and F1-score
	•	Plotted confusion matrix

⸻

🔍 Results



📊 Visuals
	•	Class distribution (fraud vs non-fraud)
	•	Confusion matrix
	•	Optional: t-SNE plot or PCA projection (if you’re feeling spicy)

⸻

🧠 What I Learned
	•	How to handle class imbalance in anomaly detection
	•	The power of Isolation Forest for unsupervised outlier detection
	•	Basic model evaluation using scikit-learn
	•	How to structure a machine learning project and push it to GitHub like a pro 😎

⸻

🌱 Future Improvements
	•	Try other models (e.g., One-Class SVM, Autoencoders)
	•	Tune contamination dynamically
	•	Deploy a basic app using Streamlit or Flask (why not dream big, love?)

⸻

💖 Credits

Made with love, caffeine, and a tiny sprinkle of anxiety
by Gowthami ✨
