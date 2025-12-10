# Final: Sentiment Analysus of IMDB Movie Reviews

## What I Did
- Used IMDB Dataset.csv from Kaggle (50,000 samples; sampled 5,000 for efficiency; positive/negative labels).
- EDA: Checked nulls (none), sentiment balance (~50/50), text lengths (avg 1,321 chars), common words, samples. Preprocessed: Lowercase, removed URLs/punctuation/numbers/spaces; created 'cleaned_text'.
- Features: TF-IDF (max_features=5,000, min_df=2, max_df=0.8, ngrams=1-2, stopwords).
- Models: Logistic Regression (max_iter=1,000), Naive Bayes, Random Forest (n_estimators=100, max_depth=20).
- Evaluated: Metrics (accuracy/precision/recall/F1), reports, confusion matrices; error analysis.

## What I Learned
- Dataset balance: 50/50 aids reliability; slight skews affect predictions..
- Preprocessing: Noise removal boosts features; bag-of-words misses context like negations.
- Model selection: Logistic Regression best (86% accuracy); Naive Bayes fast (84%); Random Forest complex but slower (83%).
  
## Challenges
- Dataset URL broken; sourced alternative from GitHub.
- Memory limits with large data; fixed via sampling/efficient params.
- Misclassifications (false negatives); suggested SMOTE/class weights.
- Sarcasm/subjectivity; noted BERT for future.
- Overall, integrated AI for deployable insights, highlighting overfitting risks.
