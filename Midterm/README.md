# MidTerm Project: Titanic Survival Data Analysis

## What I Did
- Loaded Titanic dataset (891 samples; features like Age, Sex, Class; target Survived).
- Models: Logistic Regression baseline (accuracy 79%), Random Forest (n_estimators=100, accuracy 82%).
- Evaluated: Classification report (Random Forest precision 78%/recall 74% for survived), confusion matrix; error analysis.

## What I Learned
- Gender key: Females had 70% survival—strongest predictor. Age was the second largest predictor of survival.
- Imputation: Median avoids outlier skew unlike mean/mode for missing data.
- Models: Random Forest improves over Logistic Regression by capturing interactions.
- Errors: False Negatives were worse to have, its best to over prepare for rescue.

  
## Challenges
- Encoding categories; Embarked has no hierarchy, so one-hot via get_dummies prevented ordinal assumption errors—learned that improper encoding can distort model interpretations, like assuming port order matters.
- Feature selection; dropped non-numeric/irrelevant like Name/Ticket/Cabin (high nulls), focusing on predictive ones—challenged by potential info loss, but prioritized simplicity for clear narratives.
- Error trade-off; False Negative (missed non-survivors) impacts critical decisions like resource allocation—prioritized recall over precision, reflecting ethical need to minimize harm in life-or-death predictions.
