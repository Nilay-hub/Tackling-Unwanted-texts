# 📩 Spam SMS Classification using Machine Learning

This project focuses on **automated SMS spam detection** using **Machine Learning and Natural Language Processing (NLP)** techniques. With the growing influx of spam messages, this project builds a classifier capable of distinguishing between **spam (unwanted messages)** and **ham (legitimate messages)**.

## 🚀 **Project Overview**
The objective of this project is to analyze text messages and classify them into spam or ham using **machine learning models**. The dataset consists of SMS messages labeled as either spam or ham, and various preprocessing techniques are applied before feeding the data into classification algorithms.

### **Techniques Used:**
- **Natural Language Processing (NLP)** for text processing
- **Feature Engineering** to extract key patterns from messages
- **Machine Learning Classifiers**:
  - **Multinomial Naïve Bayes**
  - **Decision Tree**
  - **Random Forest**
  - **Voting Ensemble**
- **Exploratory Data Analysis (EDA)** for data insights
- **Performance Evaluation** using metrics like F1-score, Precision, and Recall

---

## 📂 **Project Structure**
📁 Spam_SMS_Classification/ │── 📄 Spam_SMS_Collection.txt # Dataset containing SMS messages labeled as spam or ham │── 📄 Spam_SMS Classification_Research Paper.pdf # Research paper detailing the study │── 📄 README.md # Project documentation │── 📜 Spam_SMS_Classification.ipynb # Jupyter Notebook for training and evaluating models


---

## 🔧 **Setup & Execution**
### **1️⃣ Prerequisites**
Ensure you have the following installed before running the code:
- Python (>=3.8)
- Jupyter Notebook or Google Colab
- Required Python libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn nltk
2️⃣ Steps to Run the Project
Load the dataset (Spam_SMS_Collection.txt) in the Jupyter Notebook.
Run the Notebook Spam_SMS_Classification.ipynb:
Preprocess the SMS text data.
Train different classification models.
Evaluate their performance.
Analyze the results to identify the most effective spam classifier.
🛠 Data Preprocessing & Feature Engineering

The dataset is preprocessed using Natural Language Processing (NLP) techniques:

Lowercasing: Converts all text to lowercase.
Removing Special Characters: Cleans up unwanted characters.
Tokenization: Splits text into words.
Stopword Removal: Filters out common words that do not carry meaning.
Lemmatization: Converts words to their base form.
Additional features engineered:

Word Count: Number of words in the SMS.
Presence of Numbers: Checks if the message contains numbers.
Presence of Currency Symbols: Identifies possible promotional content.
📊 Machine Learning Models Used

Model	Strengths	Limitations
Multinomial Naïve Bayes	Fast and effective for text classification	Assumes independence between features
Decision Tree	Easy to interpret, handles non-linearity	Can overfit easily
Random Forest	Robust and high accuracy	Computationally expensive
Voting Ensemble	Combines multiple models for better accuracy	Complexity increases
Best Performing Model:
The Random Forest Classifier achieved the highest F1-Score of 0.994, making it the best model for spam detection.
📈 Results & Insights

Spam messages often contain numbers, currency symbols, and promotional words.
Naïve Bayes performed well with text data but lacked robustness compared to Random Forest.
Voting Ensemble was tested, but it did not outperform Random Forest.
❗ Limitations

The dataset may not generalize well to new spam trends.
Some legitimate promotional messages might be falsely classified as spam.
The model does not consider sender metadata, which could improve spam detection.
📢 Acknowledgments

This research was conducted by Nilay Nisheethkumar Patel & Pranav Reddy Bande at Georgia State University.

