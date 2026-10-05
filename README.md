# House Price Prediction using Machine Learning

## Project Overview

This project predicts house prices using Machine Learning regression algorithms. It analyzes house features such as area, bedrooms, bathrooms, age, location, and property type.

## Objectives

* Understand and preprocess housing data.
* Implement Linear Regression from scratch.
* Train a Scikit-learn Linear Regression model.
* Compare Polynomial Regression, Decision Tree, and Random Forest.
* Evaluate models using MAE, MSE, and R² Score.
* Visualize actual versus predicted prices.

## Dataset

* **Records:** 300
* **Columns:** 8
* **Target Variable:** Price
* **Features:** Area, Bedrooms, Bathrooms, Age, Location, Property Type

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
DeveloperArena-Week9/
├── house_data.csv
├── house_price_prediction.ipynb
├── predictions_vs_actual.png
├── model_results.csv
├── model_evaluation_report.md
├── requirements.txt
└── README.md
```

## Model Performance

| Model                 |             MAE | R² Score |
| --------------------- | --------------: | -------: |
| Linear Regression     |       2,188,736 |   0.9406 |
| Polynomial Regression | Approximately 0 |   1.0000 |
| Decision Tree         |       3,171,748 |   0.8791 |
| Random Forest         |       1,493,949 |   0.9711 |

Random Forest provided the best practical performance among the models evaluated. Polynomial Regression produced an unusually perfect result that may indicate overfitting and requires further validation.

## Key Findings

* Area was the most important feature, with approximately 69.32% feature importance.
* Location was another important factor.
* Random Forest achieved an R² score of approximately 97.11%.
* Actual-versus-predicted prices were visualized for model evaluation.

## Installation

Install the required libraries:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook house_price_prediction.ipynb
```

Run the notebook cells in order to reproduce the analysis.

## Conclusion

This project demonstrates how Machine Learning can predict house prices and identify important property features. Random Forest performed well on the test dataset, while additional validation is recommended before real-world use.
