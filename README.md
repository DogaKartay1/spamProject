# 📧 Spam Mail Detection with Machine Learning

A simple machine learning project that detects whether an email is **Spam** or **Ham (Not Spam)** using **Natural Language Processing (NLP)** and a **Random Forest Classifier**.

---

## 🚀 Project Overview

This project uses:

* **Python**
* **NLTK** for text preprocessing
* **Scikit-learn** for machine learning
* **CountVectorizer** for text vectorization
* **RandomForestClassifier** for classification

The dataset is cleaned, processed, converted into numerical vectors, and then used to train a spam detection model.

---

## 📂 Dataset

Dataset used:

`spam_ham_dataset[1].csv`

Expected columns:

* `text` → Email content
* `label_num` → Target label

  * `0` = Ham
  * `1` = Spam

---

## ⚙️ Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/spam-mail-detector.git
cd spam-mail-detector
```

Install dependencies:

```bash
pip install pandas numpy nltk scikit-learn
```

---

## ▶️ Running the Project

Run the Python file:

```bash
python spam_detector.py
```

---

## 🧠 How It Works

### 1. Text Cleaning

* Convert text to lowercase
* Remove punctuation
* Remove stopwords
* Apply stemming

### 2. Vectorization

Text data is converted into numerical format using:

```python
CountVectorizer()
```

### 3. Model Training

The model is trained using:

```python
RandomForestClassifier()
```

### 4. Prediction

The trained model predicts whether an email is spam or ham.

---

## 📊 Example Prediction

```python
clf.predict(x_email)
```

Output:

```python
[1]
```

* `1` → Spam
* `0` → Ham

---

## 📈 Model Performance

The model accuracy is evaluated using:

```python
clf.score(x_test, y_test)
```

---

## 📌 Features

✅ Email preprocessing
✅ Stopword removal
✅ Stemming
✅ Bag of Words model
✅ Spam/Ham classification
✅ Machine Learning pipeline

---

## 🛠 Possible Improvements

* Use **TF-IDF Vectorizer**
* Try other models:

  * Naive Bayes
  * Logistic Regression
  * XGBoost
* Add a web interface with Flask or Streamlit
* Save trained model with Pickle

---

## 📄 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

Developed by **[Doğa Kartay]**
