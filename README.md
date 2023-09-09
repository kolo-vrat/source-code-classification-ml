# Source Code Classification Using Machine Learning

This project uses a dataset derived from a [Kaggle](ttps://www.kaggle.com/datasets/simiotic/github-code-snippets-development-sample) dataset trimmed down to 84907 code snippets from nine programming languages that are collected from GitHub. The programming languages that are used are: C, C++, Python, JavaScript, Java, Go, Rust, HTML, Ruby.

### Install the required packages

The required packages are located in the requirements.txt file. You can use this command to install them.

```shell
python3 -m pip install -r requirements.txt
```

### Goal

The main goal is to train machine learning models to automatically categorize a code snippet into the correct programming language.

### Methods

The main idea was to build a vocabulary using TF-IDF(Term Frequency – Inverse Document Frequency) and Count Vectorizers and then pass it into machine learning algorithms to see which one is the best for this task. The machine learning algorithms that were used: Random Forest, Naïve Bayes, Gradient boosting methods(XGBoost and LightGBM), Logistic Regression, Voting and Stacking. 

### Results and conclusions

The acquired results are excellent. The main obstacles faced were how to get good and informative code snippets and how to find the best parameters for the vectorizers.

The evaluation metrics of the models:
| Model | Precision | Recall | F1-score | Accuracy |
| ----- | --------- | ------ | -------- | -------- |
| Random Forest | 0.94 | 0.94 | 0.94 | 0.94 |
| Random Forest (With feature selection) | 0.94 | 0.94 | 0.94 | 0.94 |
| Naïve Bayes | 0.93 | 0.92 | 0.92 | 0.92 |
| XGBoost | 0.9 | 0.9 | 0.9 | 0.89 |
| LightGBM | 0.94 | 0.94 | 0.94 | 0.94 |
| Logistic Regression | 0.94 | 0.94 | 0.94 | 0.94 |
| Voting | 0.95 | 0.95 | 0.95 | 0.95 |
| Stacking | 0.93 | 0.93 | 0.93 | 0.93 |
