# Comment Category Classifier

An end-to-end **Natural Language Processing (NLP)** project for multi-class comment classification using **TF-IDF features, structured metadata, and ensemble machine learning models**. This project focuses on building robust text classification pipelines through feature engineering, model comparison, hyperparameter tuning, and ensemble learning techniques.

The final ensemble model achieved a **Macro-F1 score of 0.81**, outperforming individual baseline models.

---

## 📌 Project Overview

Online platforms generate millions of user comments every day. Automatically categorizing these comments helps improve content moderation, recommendation systems, sentiment analysis, and user engagement analytics.

This project aims to classify user comments into **four distinct categories** using a combination of:

* Textual features
* Structured metadata
* Feature engineering
* Machine learning ensembles

The complete workflow includes:

* Exploratory Data Analysis (EDA)
* Data preprocessing
* Feature engineering
* Text vectorization
* Model training
* Hyperparameter tuning
* Ensemble learning
* Performance evaluation

---

## 📊 Dataset Information

### Training Dataset

* Approximately **198,000 samples**
* **15 features**

### Test Dataset

* Approximately **102,000 samples**
* **14 features**

### Features Included

| Feature      | Description                |
| ------------ | --------------------------- |
| comment      | User comment text          |
| created_date | Date of comment creation   |
| post_id      | Associated post identifier |
| emoticon_1   | First emoticon             |
| emoticon_2   | Second emoticon            |
| emoticon_3   | Third emoticon             |
| upvote       | Number of upvotes          |
| downvote     | Number of downvotes        |
| race         | User race information      |
| religion     | User religion information  |
| gender       | User gender information    |
| disability   | Disability status          |
| if_1         | Binary indicator           |
| if_2         | Binary indicator           |
| label        | Target class               |

---

## 🔎 Exploratory Data Analysis

Several exploratory analyses were performed, including:

* Missing value analysis
* Target label distribution
* Correlation analysis
* Numerical feature distributions
* Categorical feature distributions
* Comment length analysis
* Feature importance exploration

---

## ⚙️ Data Preprocessing

The preprocessing pipeline consisted of:

### Text Processing

* Lowercasing
* Missing value handling
* TF-IDF vectorization
* Vocabulary pruning

### Feature Engineering

* Comment length generation
* Date feature extraction:

  * Year
  * Month
  * Day
* Metadata transformation
* Categorical encoding

### Missing Value Handling

Missing values in:

* Race
* Religion
* Gender

were replaced using:

```python
"missing"
```

---

## 🧠 Feature Representation

### Text Features

* TF-IDF Vectorizer
* N-gram representation
* Sparse matrix optimization

### Structured Features

* Engagement features
* Date features
* Comment statistics
* Encoded categorical features

---

## 🤖 Models Evaluated

The following machine learning models were benchmarked:

### Logistic Regression

* Fast baseline classifier
* Strong performance on sparse text features

### Decision Tree

* Interpretable baseline model

### Random Forest

* Ensemble tree-based approach

### Multi-Layer Perceptron (MLP)

* Neural network-based classifier

### LightGBM

* Gradient boosting framework optimized for performance

---

## 🔧 Hyperparameter Tuning

Model optimization was performed using:

* GridSearchCV
* 3-Fold Cross Validation

Parameters tuned included:

* Learning rate
* Number of estimators
* Tree depth
* Regularization parameters
* Hidden layer sizes

---

## 🏆 Ensemble Learning

A soft-voting ensemble was constructed using:

* Logistic Regression
* Multi-Layer Perceptron (MLP)
* LightGBM

This ensemble achieved the best overall performance.

---

## 📈 Results

| Model                | Performance           |
| --------------------- | ---------------------- |
| Logistic Regression  | Strong Baseline        |
| Decision Tree         | Baseline                |
| Random Forest         | Moderate                |
| MLP                    | Strong                   |
| LightGBM               | Strong                   |
| Voting Ensemble       | **Best Performance**   |

### Final Performance

✅ **Macro-F1 Score: 0.81**

---

## 🛠️ Technology Stack

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* LightGBM
* Matplotlib
* Seaborn

### NLP

* TF-IDF Vectorization

### Tools

* Jupyter Notebook
* Kaggle

---

## 📁 Project Structure

```text
Notebook/

└── Comment_Category_Classifier.ipynb
```

---

## 🚀 How to Run

### Clone the Repository

```bash
git clone https://github.com/USERNAME/Comment-Category-Classifier.git

cd Comment-Category-Classifier
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Comment_Category_Classifier.ipynb
```

and execute all cells sequentially to reproduce the complete workflow, including preprocessing, feature engineering, model training, evaluation, and prediction generation.

---

## 🎯 Key Learnings

Through this project, I gained practical experience in:

* End-to-end NLP pipelines
* Text feature engineering
* TF-IDF vectorization
* Ensemble machine learning
* Hyperparameter optimization
* Cross-validation
* Feature preprocessing
* Model evaluation metrics
* Kaggle competition workflows

---

## 👨‍💻 Author

**Abhinav Raj**

BS in Data Science and Applications
Indian Institute of Technology Madras

* GitHub: https://github.com/24f1000806
* LinkedIn: https://www.linkedin.com/in/avi-raj-q01

---

⭐ If you found this project interesting, feel free to star the repository.
