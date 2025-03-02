# Payment Fraud URL Detection

## Table of Content
  * [Introduction](#introduction)
  * [Installation](#installation)
  * [Directory Tree](#directory-tree)
  * [Result](#result)
  * [Conclusion](#conclusion)

## Introduction

With the rise of online transactions, fraudulent payment URLs have become a major concern. Fraudsters create deceptive websites that imitate legitimate payment portals to steal sensitive financial information such as credit card details, banking credentials, and personal data. While various methods have been implemented to detect fraudulent payment sites, cybercriminals continue to refine their techniques to bypass detection. One of the most effective approaches for identifying fraudulent URLs is **Machine Learning**. By analyzing patterns and characteristics commonly found in fraudulent URLs, machine learning models can significantly improve fraud detection and enhance online security.

## Installation

The code is developed in Python 3.6.10. If Python is not installed, download it [here](https://www.python.org/downloads/). If using an older version, upgrade using pip to ensure compatibility. To install the required dependencies, navigate to the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository and run:

```bash
pip install -r requirements.txt
```

## Directory Tree
```
├── pickle
│   ├── model.pkl
├── static
│   ├── styles.css
├── templates
│   ├── index.html
├── Payment Fraud URL Detection.ipynb
├── Procfile
├── README.md
├── app.py
├── feature.py
├── payment_fraud_urls.csv
├── requirements.txt
```

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg" width=200>](https://numpy.org/doc/)
[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Pandas_logo.svg" width=200>](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" width=100>](https://matplotlib.org/)
[<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/)
[<img target="_blank" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScq-xocLctL07Jy0tpR_p9w0Q42_rK1aAkNfW6sm3ucjFKWML39aaJPgdhadyCnEiK7vw&usqp=CAU" width=200>](https://flask.palletsprojects.com/en/2.0.x/)

## Result

Accuracy of different models used for detecting fraudulent payment URLs:

||ML Model| Accuracy| f1_score| Recall| Precision|
|---|---|---|---|---|---|
0| Gradient Boosting Classifier| 0.974| 0.977| 0.994| 0.986|
1| CatBoost Classifier| 0.972| 0.975| 0.994| 0.989|
2| XGBoost Classifier| 0.969| 0.973| 0.993| 0.984|
3| Multi-layer Perceptron| 0.969| 0.973| 0.995| 0.981|
4| Random Forest| 0.967| 0.971| 0.993| 0.990|
5| Support Vector Machine| 0.964| 0.968| 0.980| 0.965|
6| Decision Tree| 0.960| 0.964| 0.991| 0.993|
7| K-Nearest Neighbors| 0.956| 0.961| 0.991| 0.989|
8| Logistic Regression| 0.934| 0.941| 0.943| 0.927|
9| Naive Bayes Classifier| 0.605| 0.454| 0.292| 0.997|

Feature importance for Payment Fraud URL Detection:

![image](https://user-images.githubusercontent.com/79131292/144603941-19044aae-7d7b-4e9a-88a8-6adfd8626f77.png)

## Conclusion

1. This project explores various machine learning models to detect fraudulent payment URLs, perform **Exploratory Data Analysis (EDA)** on the dataset, and understand the features affecting classification accuracy.
2. By analyzing key features influencing model performance, we gain insights into critical indicators of fraudulent payment URLs.
3. Features such as "HTTPS usage," "AnchorURL patterns," and "Website Traffic" significantly impact classification accuracy.
4. The **Gradient Boosting Classifier** achieved the highest accuracy of **97.4%**, making it the most effective model for identifying fraudulent payment URLs, thereby enhancing online transaction security.

# payment-fraud-url-detection

