# Task 4 · Email Spam Detection with Machine Learning

**Track:** Data Science
**Internship:** Oasis Infobyte SIP

## Objective
Build a Natural Language Processing (NLP) binary classifier that distinguishes spam messages from legitimate (ham) messages, using classic NLP feature engineering and machine learning classifiers.

## Dataset
- **Source:** SMS Spam Collection Dataset (originally hosted on the UCI Machine Learning Repository / Kaggle)
- **Size:** 5,572 SMS messages (5,169 after removing duplicates)
- **Labels:** `ham` (legitimate, ~87%) and `spam` (~13%)
- **File:** `spam_data.csv` (columns: `label`, `message`)

## Tech Stack
- Python
- pandas, numpy
- NLTK (stopword removal)
- scikit-learn (TF-IDF Vectorizer, Multinomial Naive Bayes, Logistic Regression, evaluation metrics)
- matplotlib, seaborn, WordCloud
- Jupyter Notebook

## Approach
1. **Data loading & cleaning** — loaded the dataset, checked for nulls/duplicates, removed duplicate messages.
2. **Class distribution check** — confirmed the dataset is imbalanced (~87% ham / ~13% spam) and discussed why this matters for evaluation.
3. **Text preprocessing pipeline** — lowercasing, punctuation removal, digit removal, and stopword removal.
4. **WordCloud visualisations (bonus)** — compared the most frequent words in spam vs. ham messages.
5. **Feature extraction** — TF-IDF Vectorizer (max 3,000 features), with a markdown explanation of what TF-IDF measures.
6. **Train/test split** — 80/20 stratified split.
7. **Model training** — trained two classifiers:
   - Multinomial Naive Bayes (industry-standard baseline for text)
   - Logistic Regression (alternative linear model)
8. **Evaluation** — accuracy, precision, recall, F1-score, and confusion matrices for both models.
9. **Discussion** — a written explanation of why **recall** is particularly important for spam detection (missed spam can mean missed phishing/scam attempts, not just clutter).
10. **Error analysis** — inspected a sample of misclassified messages.

## Results Summary
Both models achieve strong performance on the held-out test set (>95% accuracy), with Naive Bayes and Logistic Regression showing different precision/recall trade-offs on the minority (spam) class. See the notebook for exact metrics, confusion matrices, and the full discussion.

## Files in this folder
- `email_spam_detection.ipynb` — full, executed Jupyter Notebook with all steps, visualisations, and markdown commentary
- `spam_data.csv` — the dataset used
- `README.md` — this file

## How to Run
1. Download `email_spam_detection.ipynb` and `spam_data.csv` into the same folder.
2. Install dependencies: `pip install pandas numpy scikit-learn nltk matplotlib seaborn wordcloud`
3. Launch Jupyter: `python -m notebook`
4. Open the notebook and select **Kernel → Restart & Run All**.
