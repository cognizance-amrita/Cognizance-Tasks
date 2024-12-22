# AI Domain

**Authors:** Shalini D and Jeba Rachel

---

## Task 1: Model Selection for Regression with Scikit-learn

### Objective:
Build a regression model to predict diabetes progression using Scikit-learn. This task will help you understand the fundamentals of selecting and evaluating regression models.

### Dataset:
Diabetes Dataset (available in Scikit-learn).

---

### Steps

1. **Load the Dataset**  
   - Use Scikit-learn to load the Diabetes dataset.  
   - Convert it into a Pandas DataFrame for preprocessing.  

   **Code:**  
   ```python
   from sklearn.datasets import load_diabetes
   import pandas as pd
   data = load_diabetes()
   df = pd.DataFrame(data.data, columns=data.feature_names)
   df['progression'] = data.target
   df.to_csv("diabetes.csv", index=False)
   ```

2. **Preprocess the Data**  
   - Load the CSV file using Pandas.  
   - Check for missing values and handle them if present.  
   - Standardize numerical features using `StandardScaler`.  

3. **Model Selection**  
   - Compare multiple regression models, such as Linear Regression, Ridge Regression, and Random Forest Regressor.  
   - Use cross-validation to evaluate model performance using Mean Squared Error (MSE).  

4. **Train and Test the Best Model**  
   - Split the data into training and testing sets (80-20 split).  
   - Train the selected model on the training set.  
   - Evaluate its performance on the test set.  

---

### Deliverables

- A Google Colab Notebook containing:  
  - Code for data preprocessing, model comparison, and evaluation.  
  - Comments explaining each step.  
  - A summary of the best model and its MSE on the test set.  

---

## Task 2: Model Selection for Classification with Scikit-learn

### Objective:
Build a classification model to predict iris species using Scikit-learn. This task focuses on understanding the process of selecting the best classification model.

### Dataset:
Iris Dataset (available in Scikit-learn).

---

### Steps

1. **Load the Dataset**  
   - Use Scikit-learn to load the Iris dataset.  
   - Convert it into a Pandas DataFrame for preprocessing.  

   **Code:**  
   ```python
   from sklearn.datasets import load_iris
   import pandas as pd
   data = load_iris()
   df = pd.DataFrame(data.data, columns=data.feature_names)
   df['species'] = data.target
   df.to_csv("iris.csv", index=False)
   ```

2. **Preprocess the Data**  
   - Load the CSV file in Pandas.  
   - Handle missing values if present.  
   - Standardize numerical features using `StandardScaler`.  
   - Encode the target variable using label encoding.  

3. **Model Selection**  
   - Compare multiple classification models, such as Logistic Regression, Decision Trees, and Support Vector Machines (SVM).  
   - Use cross-validation to evaluate model performance using accuracy and F1-score.  

4. **Train and Test the Best Model**  
   - Split the data into training and testing sets (80-20 split).  
   - Train the selected model on the training set.  
   - Evaluate its performance on the test set.  

---

### Deliverables

- A Google Colab Notebook containing:  
  - Code for data preprocessing, model comparison, and evaluation.  
  - Comments explaining each step.  
  - A summary of the best model and its accuracy and F1-score on the test set.  

---

## References

### General References:
1. **Regression:**  
   - [Scikit-learn Regression Guide](https://scikit-learn.org/stable/supervised_learning.html#supervised-learning)  
   - [StandardScaler Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)  

2. **Classification:**  
   - [Scikit-learn Classification Guide](https://scikit-learn.org/stable/supervised_learning.html#classification)  
   - [Cross-validation](https://scikit-learn.org/stable/modules/cross_validation.html)  

### Specific Techniques:
- **Data Splitting:** [Train-Test Split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html)  
- **Handling Missing Values:** [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.fillna.html)  
- **Model Selection:** [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)  

---

**Note:** Complete each task in Google Colab and upload your notebooks to your GitHub profile.

