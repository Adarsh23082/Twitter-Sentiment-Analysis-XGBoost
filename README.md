# Twitter Sentiment Analysis using XGBoost

## 📝 Project Overview

This project performs **sentiment analysis on tweets** using Natural Language Processing (NLP) techniques and machine learning models. The primary goal is to classify the emotional tone of tweets into categories like **positive**, **negative**, **neutral**, or **irrelevant**. The pipeline includes data cleaning, feature extraction using TF-IDF, and classification using models like **Multinomial Naive Bayes** and **XGBoost**.

This project highlights how real-time text data can be transformed into insights about public sentiment, which is valuable for brand monitoring, customer feedback analysis, or social media trend tracking.

---

## 📂 Dataset

The project uses two datasets:

- `twitter_training.csv`: Contains labeled tweets for model training.
- `twitter_validation.csv`: Used to validate model performance on unseen data.

Each dataset includes the following columns:
- `id`: Unique identifier for each tweet.
- `information`: Additional meta info (not used in modeling).
- `type`: Emotion or sentiment label (e.g., Positive, Negative, Neutral, Irrelevant).
- `text`: The tweet content.

---

## 🛠 Tools and Libraries Used

- **Python 3**
- **Pandas** for data manipulation
- **Matplotlib** for visualization
- **NLTK** for tokenization, stopword removal, and preprocessing
- **Scikit-learn** for TF-IDF vectorization, model training, and evaluation
- **XGBoost** for robust classification

---

## 🔍 Key Steps & Methodology

1. **Data Cleaning & Preprocessing:**
   - Removed null entries and cleaned text (lowercased, removed URLs and special characters).
   - Tokenized and removed stopwords using NLTK.

2. **Feature Engineering:**
   - Used **TF-IDF Vectorizer** to convert textual data into numerical features for modeling.

3. **Model Training:**
   - Trained both **Multinomial Naive Bayes** and **XGBoost** classifiers.
   - Used `train_test_split` for model validation and testing.

4. **Model Evaluation:**
   - Evaluated using metrics like **accuracy**, **confusion matrix**, and **classification report**.
   - Visualized sentiment distribution using **pie charts**.

---

## 📈 Key Insights

- The training dataset is imbalanced, with **Positive and Negative tweets** dominating.
- Text preprocessing significantly improved model performance.
- **XGBoost** outperformed the Naive Bayes model, delivering higher accuracy and better classification metrics.
- Certain keywords strongly correlated with specific sentiments, highlighting the effectiveness of TF-IDF.

---

## 💡 Recommendations

1. Use **SMOTE or class-weight adjustment** to handle class imbalance for better generalization.
2. Extend the model to support **multi-language tweets** with language detection and translation.
3. Explore **deep learning models** like LSTM or BERT for potentially higher accuracy.
4. Deploy the model using **Flask or FastAPI** for real-time sentiment analysis applications.

---

## 📁 Folder Structure

