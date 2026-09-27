\# DSN Mart Sales Prediction



Machine learning solution for the DSN AI Bootcamp 2026 Qualification Hackathon — ML Track.



\## Competition



The task was to predict product-store `total\_sales` using product and store characteristics.



\## Results



\- 5-fold cross-validation RMSE: \*\*1072.30\*\*

\- Kaggle leaderboard RMSE: \*\*1074.00044\*\*



\## Approach



The project covers:



\- Exploratory data analysis

\- Missing-value analysis

\- Categorical feature analysis

\- Feature engineering

\- CatBoost model development

\- Hyperparameter tuning

\- Cross-validation

\- Target decomposition



\### Target decomposition



The final modeling approach decomposed sales into:



`total\_sales = product\_price × units\_sold`



The model was trained to predict `units\_sold`, after which predicted sales were reconstructed using product price.



\### Model



The final CatBoost model used:



\- 500 iterations

\- Learning rate: 0.02

\- Depth: 4

\- L2 leaf regularization: 12

\- Random strength: 2

\- 5-fold KFold cross-validation

\- Random seed: 42



\## Competition Result



Final Kaggle leaderboard RMSE:



\*\*1074.00044\*\*

