Markdown

# 📰 Fake News Detection System

![Python](https://img.shields.io/badge/Python-3.12%2B-blue)
![Flask](https://img.shields.io/badge/Framework-Flask-green)
![ML](https://img.shields.io/badge/AI-Scikit_Learn-orange)
![License](https://img.shields.io/badge/License-Academic-lightgrey)

**CSC3600 Project** is a Machine Learning-based web application developed to classify news articles as **Fake News** or **Not a Fake News (Real)**.

The system applies **Natural Language Processing (NLP)** techniques and evaluates text using **four ensemble machine learning models** to ensure high reliability and accuracy.

---

## 🚀 Key Features

* 🔍 **Multi-Model Prediction:** simultaneously verifies news using 4 algorithms:
    * Logistic Regression
    * Decision Tree Classifier
    * Gradient Boosting Classifier
    * Random Forest Classifier
* 🔗 **URL-Based Detection:** Built-in web scraper (using **BeautifulSoup**) extracts text directly from news links.
* 🧹 **Smart Preprocessing:** Automatically cleans input text (removes URLs, punctuation, special characters) using RegEx.
* 📊 **Performance Metrics:** Evaluates models based on Accuracy, Precision, Recall, and F1 Score.

---

## 🛠️ Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Backend** | Python (Flask) | Web server and API handling. |
| **Machine Learning** | Scikit-Learn | Model training and prediction. |
| **Data Processing** | Pandas | Handling `True.csv` and `Fake.csv` datasets. |
| **NLP** | TF-IDF Vectorizer | Converting text into numerical feature vectors. |
| **Web Scraping** | BeautifulSoup (bs4) | Extracting article content from URLs. |

---

## 📂 Project Structure

```text
CSC3600Project/
├── app2.py              # Main Flask Application
├── Fake.csv             # Dataset (Fake News)
├── True.csv             # Dataset (Real News)
├── templates/
│   ├── index.html       # Web Interface
│   └── index2.html      # Alternate Interface
└── README.md
⚙️ Installation & Setup
1. Clone the Repository
Bash

git clone [https://github.com/hannbella18/CSC3600Project.git](https://github.com/hannbella18/CSC3600Project.git)
cd CSC3600Project
2. Install Dependencies
Bash

pip install flask pandas scikit-learn requests beautifulsoup4
3. Run the Application
Bash

python app2.py
The application will launch at http://127.0.0.1:5000/

🧠 Model Details
🔹 Text Vectorization
Uses TF-IDF (Term Frequency-Inverse Document Frequency) to transform raw text into meaningful numerical features for the AI.

🔹 Dataset Handling
Combines Fake.csv and True.csv.

Uses a 10% random sample of the data during training to ensure fast performance.

🔹 Algorithms Used
Logistic Regression: Baseline model for binary classification.

Decision Tree: Captures non-linear data patterns.

Gradient Boosting: Ensemble technique that optimizes predictive errors.

Random Forest: Reduces overfitting by averaging multiple decision trees.

👤 Author
Hannbella

Computer Science Student @ UPM

GitHub Profile

📄 License
This project is developed for academic purposes under the CSC3600 course.
