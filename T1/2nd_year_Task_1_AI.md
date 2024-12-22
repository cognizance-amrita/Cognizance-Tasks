
**<span style="color: #90EE9; font-size: 1.5rem;">AI Domain</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Authors - Jagaadhep U K and Ragi Pranav</span>**

---

**<span style="color: #FF6363; font-size: 1rem;">Task 1: Supervised Learning with TensorFlow</span>**

**<span style="color: #ADD8E6;">Objective:</span>**  
Build a deep learning classification model to predict heart disease risk. This task will help you understand the fundamentals of building a deep learning pipeline using TensorFlow, preprocessing data, training a model, and evaluating its performance.  

Supervised learning involves training a model on labeled data, where the objective is to learn the mapping from input features to a target output. This task emphasizes the use of TensorFlow for building and training a deep learning model.  

**<span style="color: #ADD8E6;">Dataset:</span>**  
Heart Disease Dataset (available in TensorFlow Datasets, converted to CSV).  

---

**<span style="color: #ADD8E6;">Steps</span>**

1. **Load the Dataset**  
   - Load the Heart Disease dataset from TensorFlow Datasets.  
   - Convert it into CSV format for preprocessing.  

   **Code:**  
   ```python
   import tensorflow_datasets as tfds  
   import pandas as pd  
   ds = tfds.load('heart', split='train', as_supervised=False)  
   df = tfds.as_dataframe(ds)  
   df.to_csv("heart_disease.csv", index=False)  
   ```  

2. **Preprocess the Data**  
   - Load the CSV file using Pandas.  
   - Handle missing values.  
   - Normalize numerical features.  
   - Encode categorical variables using one-hot encoding.  

3. **Build and Train a Deep Learning Model**  
   - Define a TensorFlow Sequential model with:  
     - Dense layers with ReLU activation.  
     - Output layer with sigmoid activation for binary classification.  
   - Compile the model with `binary_crossentropy` loss and the Adam optimizer.  
   - Train the model using the training set for 20 epochs with a batch size of 32.  

4. **Evaluate the Model**  
   - Split the data into training and testing sets (80-20 split).  
   - Evaluate the model's performance using accuracy and F1-score on the test set.  

---

**<span style="color: #ADD8E6;">Deliverables</span>**  

- A Google Colab Notebook containing:  
  - Code for data preprocessing, model creation, training, and evaluation.  
  - Comments explaining each step.  
  - A summary of the model’s accuracy and F1-score.  

---
---

**<span style="color: #FF6363; font-size: 1rem;">Task 2: Unsupervised Learning with Scikit-learn</span>**

**<span style="color: #ADD8E6;">Objective:</span>**  
Perform clustering on wine quality data to group samples based on their physicochemical properties. This task focuses on understanding clustering, an unsupervised learning technique where data is grouped into clusters based on feature similarity.  

**<span style="color: #ADD8E6;">Dataset:</span>**  
Wine Quality Dataset (from Scikit-learn, converted to CSV).  

---

**<span style="color: #ADD8E6;">Steps</span>**

1. **Load the Dataset**  
   - Use Scikit-learn to load the Wine Quality dataset and save it as a CSV file.  

   **Code:**  
   ```python
   from sklearn.datasets import fetch_openml  
   import pandas as pd  
   data = fetch_openml(name='wine-quality-red', as_frame=True)  
   df = pd.concat([data.data, data.target.rename('quality')], axis=1)  
   df.to_csv("wine_quality.csv", index=False)  
   ```  

2. **Preprocess the Data**  
   - Load the CSV file in Pandas.  
   - Standardize the features using StandardScaler to ensure all features are on the same scale.  

3. **Apply KMeans Clustering**  
   - Set the number of clusters to 3.  
   - Use Scikit-learn’s KMeans algorithm to cluster the data.  

4. **Visualize the Clusters**  
   - Use a scatter plot to visualize two features (e.g., alcohol and acidity) and color-code the clusters.  

---

**<span style="color: #ADD8E6;">Deliverables</span>**  

- A Google Colab Notebook containing:  
  - Code for data preprocessing and clustering.  
  - Comments explaining each step.  
  - Visualizations of the clusters.  

---

**<span style="color: #ADD8E6;">References</span>**

**General References:**  
1. **Supervised Learning:**  
   - [TensorFlow Datasets: Documentation](https://www.tensorflow.org/datasets)  
   - [Deep Learning for Beginners: Google Colab Guide](https://colab.research.google.com/)  
   - [Preprocessing Data in TensorFlow: YouTube Tutorial](https://www.youtube.com/)  
   - [Binary Classification with TensorFlow: Guide](https://www.tensorflow.org/tutorials/structured_data/feature_columns)  

2. **Unsupervised Learning:**  
   - [Scikit-learn Clustering Guide: Documentation](https://scikit-learn.org/stable/modules/clustering.html)  
   - [Data Scaling Techniques: Kaggle Tutorial](https://www.kaggle.com/code/)  

**Specific Techniques:**  
- **Data Splitting:** [Train-Test Split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html)  
- **Handling Missing Values:** [YouTube Guide](https://www.youtube.com/)  
- **Scaling Data:** [StandardScaler vs MinMaxScaler](https://scikit-learn.org/stable/modules/preprocessing.html)  

---

**Note:** Complete each task in Google Colab and upload your notebooks to your GitHub profile.
