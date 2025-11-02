# Students Distraction & Social Media Addiction Analysis

This notebook explores the relationship between social media usage and various factors among students, including academic performance, addiction score, sleep hours, and mental health. The analysis involves data loading, visualization, correlation analysis, and building machine learning models to predict key outcomes.

## Key Findings:

### Correlation Analysis

*   Strong positive correlations were observed between average daily social media usage hours and addicted score (~0.83), addicted score and conflicts over social media (~0.93), and mental health score and sleep hours per night (~0.71).
*   Strong negative correlations were found between average daily usage hours and sleep hours per night (~0.79), average daily usage hours and mental health score (~0.80), and addicted score and mental health score (~0.95).

These correlations suggest significant relationships between social media usage, sleep, mental health, conflicts, and addiction score.

### Prediction Model Performance

The following predictive models were trained and evaluated:

#### Affects Academic Performance (Classification Model)

*   **Accuracy:** 1.0000
*   **Precision:** 1.0000
*   **Recall:** 1.0000
*   **F1-score:** 1.0000

*Interpretation:* The classification model achieved perfect scores, suggesting that the features in the dataset are highly predictive of whether social media usage affects academic performance. However, perfect scores on a test set can sometimes indicate potential issues like data leakage or a dataset where the target variable is very easily separable based on the features. Further investigation might be needed in a real-world scenario to confirm these results on unseen data.

#### Addicted Score (Regression Model)

*   **Mean Squared Error (MSE):** 0.1045
*   **R-squared:** 0.9582

*Interpretation:* The regression model for Addicted Score shows a very low Mean Squared Error (MSE) and a very high R-squared value. This indicates that the model's predictions are very close to the actual Addicted Scores, and a large proportion of the variance in Addicted Score is explained by the features. The model appears to perform exceptionally well in predicting the addicted score.

#### Sleep Hours Per Night (Regression Model)

*   **Mean Squared Error (MSE):** 0.3103
*   **R-squared:** 0.7102

*Interpretation:* The regression model for Sleep Hours Per Night has a relatively low Mean Squared Error (MSE) and an R-squared value of approximately 0.71. This means the model explains about 71% of the variance in sleep hours. While not perfect, this indicates a reasonably good fit and that the features are useful in predicting the number of sleep hours per night.

#### Mental Health Score (Regression Model)

*   **Mean Squared Error (MSE):** 0.0681
*   **R-squared:** 0.9433

*Interpretation:* The regression model for Mental Health Score shows a very low Mean Squared Error (MSE) and a high R-squared value. Similar to the Addicted Score model, this suggests that the model is highly effective in predicting the Mental Health Score based on the given features, explaining a large portion of the variance.
