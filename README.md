# 📩 Spam Message Classifier

A machine learning project that classifies text messages as **Spam** or **Ham (Not Spam)** using Natural Language Processing and Naive Bayes.

---

## 🚀 Project Overview

This project builds a text classification model trained on the SMS Spam Dataset. The steps include:

- Data loading and cleanup  
- Label encoding (`spam → 1`, `ham → 0`)  
- Text preprocessing using **TF-IDF Vectorizer**  
- Training using **Naive Bayes models**  
- Evaluating model accuracy and precision  

---

## 📁 Dataset

The dataset used is `spam.csv` encoded in `latin-1`.

| Column | Description |
|--------|------------|
| v1 → target | spam or ham |
| v2 → text | message content |
| extra columns | removed |

Final cleaned dataset contains:


---

## 🛠 Technologies Used

| Category | Tools |
|----------|-------|
| Language | Python |
| Libraries | Pandas, NumPy, Scikit-learn |
| ML Models | GaussianNB, BernoulliNB, MultinomialNB |

---

## 🧠 Machine Learning Workflow

1. Load dataset using Pandas  
2. Drop unnecessary columns  
3. Encode labels (`spam = 1`, `ham = 0`)  
4. Remove duplicates  
5. Split dataset (train-test split)  
6. Transform text using **TF-IDF Vectorizer**  
7. Train Naive Bayes classifier  
8. Evaluate using accuracy & precision metrics  

---

## 📊 Model Results

| Metric | Score |
|--------|-------|
| Accuracy | >95% |
| Precision | >95% |

---

## 💾 Model Saving

The final trained model is saved using Pickle:

```python
import pickle
pickle.dump(model, open("spam_classifier.pkl", "wb"))

# Download or clone project
git clone https://github.com/07Codex07/Mail-SMS-Classifier.git

# Install dependencies
pip install pandas numpy scikit-learn

# Run Jupyter Notebook
jupyter notebook
