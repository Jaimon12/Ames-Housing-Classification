#Ames Housing Classification

A binary classification machine learning project built on the Ames Housing dataset. This project transforms a traditional regression problem into a classification task by categorizing homes as either high-priced or low-priced based on the median sale price.

🧠 Objective

To classify houses into high or low price classes using early-known features. This enables:

Faster decisions in real estate workflows

Insight into factors that influence home prices

A foundation for automated pricing tools

📁 Dataset

Source: Ames Housing Dataset - UCI Machine Learning Repository

80 explanatory variables

2930 property transactions in Ames, Iowa

Features include physical characteristics, quality scores, location, and more

Target Variable: PriceClass

1: SalePrice > Median

0: SalePrice ≤ Median

🛠️ Methodology

Cleaned missing data and encoded categorical features

Dropped target leakage columns (e.g., SalePrice after binarization)

Trained three classifiers:

Logistic Regression

Random Forest

XGBoost

Evaluated using Accuracy, Precision, Recall, F1, and AUC

Extracted top features based on tree-based importance

📊 Results (XGBoost)

Metric

Score

Accuracy

0.90

Precision

0.91

Recall

0.88

F1 Score

0.89

AUC

0.94

Top Features:

OverallQual

GrLivArea

GarageCars

TotalBsmtSF

Neighborhood

🧐 Insights

Homes with high overall quality, large above-ground living area, and more garage space are typically high-priced.

Location (Neighborhood) plays a strong role in value.

Simpler models like logistic regression work but lack the predictive power of ensemble methods.

🧭 Next Steps

Use SHAP/LIME for model explainability

Expand dataset to multi-class classification (Low, Mid, High, Luxury)

Build dashboards to serve real estate agents or buyers interactively

📎 Files

ames_classification.ipynb – Jupyter Notebook with full code

report.pdf – PDF summary of methodology, results, and findings

README.md – Project overview

📄 License

MIT License

🤝 Contributions

Open to improvements! Feel free to fork, suggest improvements, or contribute new models.

💡 Inspiration

"Great predictions start with great questions."

