## 🚢 Titanic Survival Prediction (Kaggle Project)

This project focuses on predicting whether a passenger survived the sinking of the **RMS Titanic** using machine learning techniques. It is formulated as a **binary classification problem**, where the target variable indicates survival (`1`) or non-survival (`0`).

---

## 📊 Project Workflow

The analysis follows a complete **machine learning workflow**:

* **Exploratory Data Analysis (EDA)**
  Analyze feature distributions, relationships, and patterns in the dataset.

* **Data Preprocessing**
  Handle missing values and prepare the dataset for modeling.

* **Feature Engineering**
  Encode categorical variables, create new features, and transform existing ones to improve model performance.

* **Model Training and Evaluation**
  Train multiple models and evaluate them using appropriate performance metrics.

* **Model Comparison**
  Compare different machine learning algorithms to identify the best-performing model.


---

## 📁 Dataset

The dataset is sourced from the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic).

### Training Set

* 891 observations
* 11 input features
* 1 target variable (`Survived`)
* Total: 12 columns

### Test Set

* 418 observations
* 11 input features (same as training set)
* No target variable (to be predicted)

---

## 🧹 Data Preprocessing

* **Duplicates**
  No duplicate records were found.

* **Missing Values**

  **Training set**:

  * `Age` – filled with median
  * `Cabin` – dropped due to a large number of missing values
  * `Embarked` – filled with mode

  **Test set**:

  * `Age` – filled with median
  * `Fare` – filled with median
  * `Cabin` – dropped

* **Irrelevant Columns**

  * `Ticket` was dropped due to high diversity and limited predictive value.

* **Other Preprocessing**

  * After analysis, additional preprocessing like handling outliers or correcting data types was not required.

---

## 🔧 Feature Engineering

* **Binary Encoding**

  * `Sex` column was binary encoded as Male: `1`, Female: `0`.

* **One-Hot Encoding**

  * `Embarked` has three categories: S, Q, C; one-hot encoding was applied.

* **New Features**

  * Extracted titles from the `Name` column as a new feature.
  * Created `FamilySize` and `IsAlone` by combining `SibSp` and `Parch`.

* **Feature Transformation**

  * `Age` was binned into five categories.
  * `Fare` was scaled using `StandardScaler` from `sklearn`.

---

## 🧪 Train/Validation Split

The training dataset was split into **training** and **validation** sets in an 80:20 ratio to evaluate model performance. The test set was used for final predictions.

---

## 🤖 Models Used

The following models were applied for binary classification:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Naive Bayes
* Decision Tree
* Random Forest Classifier
* Support Vector Machine (SVC)
* Gradient Boosting Classifier
* XGBoost Classifier
* Neural Network implemented with **TensorFlow**

---

## 🏆 Skills Demonstrated

This project showcases practical machine learning workflow:

* Data Analysis (EDA)
* Data Preprocessing
* Feature Engineering
* Classification Modeling
* Model Evaluation
* Neural Networks with **TensorFlow**

---

## 📈 Results

1. **Basic preprocessing & feature engineering**

   * Handling missing values, one-hot encoding
   * Models: Logistic Regression, KNN, Naive Bayes, Decision Tree
   * Accuracy: **0.72**

2. **Scaling and Neural Network**

   * Scaling `Fare` and adding a Neural Network
   * Accuracy: **0.72**

3. **Adding new features**

   * Features: `Title`, `IsAlone`, `FamilySize`
   * Accuracy: **0.75**

4. **Advanced models**

   * Models: Random Forest, Gradient Boosting, XGBoost
   * Accuracy: **0.77**

5. **Feature transformation (Age bins)**

   * Accuracy: **0.77**

---

## ⚙️ Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* TensorFlow
* XGBoost
* Jupyter Notebook

---

## 📌 Notes

* This project is part of a popular beginner competition on Kaggle.
* It demonstrates an **end-to-end machine learning workflow** and best practices.

---
 