**<span style="color: #90EE90; font-size: 1.5rem;">AI</span>**
**<span style="color: #ADD8E6; font-size: 1rem;">Authors - R. Pranav and Jagaadhep U K</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Google Colab</span>**

Google Colab is a free online tool that lets you write and run Python code right in your web browser. It's like a notebook where you can type your code and see the results immediately. Colab is great for learning and working on data science projects because it supports popular Python libraries like Pandas and TensorFlow. You can also use it with others, making it easy to collaborate on projects. Plus, it provides access to powerful computers (GPUs and TPUs) for faster processing, which is really helpful for running complex tasks.

**Note: Use Google Colab to complete the tasks provided. After completing the tasks, upload your Google Colab Notebook to your GitHub repository.**

<span style="color: #ADD8E6;">_References:_</span>
- [<span style="color: #55AAFF;">Google Colab tutorial</span>](https://www.youtube.com/watch?v=rsBiVxzmhG0)

<hr>

**<span style="color: #FF6363; font-size: 1rem;">Question 1</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Numpy</span>**

NumPy is a popular Python library used for working with numbers and arrays. Think of it as a tool that helps you do math and handle large sets of numbers easily. It makes it simple to perform calculations on lists of numbers and matrices. NumPy is great for anyone who wants to do data analysis or scientific computing because it speeds up these tasks with its fast and powerful features.

**<span style="color: #ADD8E6; font-size: 1rem;">DataSet</span>**

We use a dataset of details about 15 students each having attributes – Height, Weight, Age, Average Grade and Courses. We use the python code given below to create a NumPy array of our dataset.

**Python code to create NumPy array for the task:**

```lua

import numpy as np
# Creating a dataset with 15 students and 5 attributes
data = np.array([
    [170, 65, 19, 85, 5],
    [180, 75, 20, 90, 6],
    [160, 55, 18, 80, 4],
    [175, 70, 21, 88, 7],
    [155, 50, 19, 82, 5],
    [165, 62, 22, 89, 6],
    [178, 80, 23, 91, 7],
    [162, 58, 20, 78, 3],
    [172, 68, 19, 86, 5],
    [169, 66, 20, 84, 4],
    [171, 64, 22, 87, 6],
    [177, 72, 21, 90, 9],
    [174, 76, 24, 88, 8],
    [158, 52, 18, 75, 3],
    [164, 63, 19, 81, 4]
])

# Printing the dataset with student labels
print("Student\tHeight\tWeight\tAge\tAvg Grade\tCourses")
for index, student in enumerate(data):
    print(f"Student {index + 1}\t{student[0]}\t{student[1]}\t{student[2]}\t{student[3]}\t\t{student[4]}")
    
```

<span style="color: #ADD8E6;">_Objective:_</span>
- <span style="color: #FF6363;">Question 1.1 : </span>Find the Average Height of the Students
  
    Explanation: You need to use the mean() function from NumPy to compute the average value of the height column in the dataset.

- <span style="color: #FF6363;">Question 1.2 : </span>Find the Age of the Oldest Student

    Explanation: Use the max() function from NumPy to find the maximum value in the age column and determine the age of the oldest student.

- <span style="color: #FF6363;">Question 1.3 : </span>Find the Index of the Student Who Took the Most Courses

    Explanation: Use the argmax() function from NumPy to locate the index of the maximum value in the number of courses column.

- <span style="color: #FF6363;">Question 1.4 : </span>Find the Number of Students with an Average Grade Above 85

    Explanation: Use a NumPy condition to filter the dataset for students with an average grade above 85, and then use the sum() function to count them.

- <span style="color: #FF6363;">Question 1.5 : </span>Calculate the Ratio of a Student's Age to Their Average Grade for Each Student

    Explanation: Perform element-wise division of the age column by the average grade column to get the ratio for each student.
  
<span style="color: #ADD8E6;">_References:_</span>
- [<span style="color: #55AAFF;">W3Schools</span>](https://www.w3schools.com/python/numpy/default.asp)
- [<span style="color: #55AAFF;">Numpy Documentation</span>](https://numpy.org/doc/stable/reference/arrays.ndarray.html)
- [<span style="color: #55AAFF;">GeeksforGeeks</span>]( https://www.geeksforgeeks.org/numpy-tutorial/)
- [<span style="color: #55AAFF;">NumPy cheat sheet</span>](https://images.datacamp.com/image/upload/v1676302459/Marketing/Blog/Numpy_Cheat_Sheet.pdf)

<hr>

**<span style="color: #FF6363; font-size: 1rem;">Question 2</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Pandas</span>**

Pandas is a powerful open-source data analysis and manipulation library for Python. It provides data structures like Data Frames and Series that are built on top of NumPy arrays and are designed to handle a wide range of data types and operations efficiently. Pandas is extensively used in data science and machine learning for tasks such as data cleaning, transformation, and analysis.

**<span style="color: #ADD8E6; font-size: 1rem;">DataSet</span>**

*We will use a dataset with 15 students, each having 5 attributes. Let's first convert the list into a Pandas DataFrame.*
```lua
data = [
    [170, 65, 19, 85, 5],
    [180, 75, 20, 90, 6],
    [160, 55, 18, 80, 4],
    [175, 70, 21, 88, 7],
    [155, 50, 19, 82, 5],
    [165, 62, 22, 89, 6],
    [178, 80, 23, 91, 7],
    [162, 58, 20, 78, 3],
    [172, 68, 19, 86, 5],
    [169, 66, 20, 84, 4],
    [171, 64, 22, 87, 6],
    [177, 72, 21, 90, 9],
    [174, 76, 24, 88, 8],
    [158, 52, 18, 75, 3],
    [164, 63, 19, 81, 4]
]
# column names being ‘Height’, ‘Weight’, ‘Age’, ‘Avg_Grade’ and ‘Courses’ in that order.
```
<span style="color: #ADD8E6;">_Objective:_</span>
- <span style="color: #FF6363;">Question 2.1 : </span>Create a Pandas DataFrame

    Explanation: You need to understand how to convert a NumPy array into a DataFrame and assign column names.

- <span style="color: #FF6363;">Question 2.2 : </span>Describe the DataFrame

    Explanation: The describe() function provides various summary statistics (mean, standard deviation, min, max, and percentiles) for numeric columns in the DataFrame.

- <span style="color: #FF6363;">Question 2.3 : </span>Count the Number of Students in Each Age Group

    Explanation: Use the value_counts() function to count occurrences of unique values in a column.

- <span style="color: #FF6363;">Question 2.4 : </span>Filter the DataFrame

  Explanation: Filtering allows you to extract specific rows from the DataFrame based on certain conditions.

- <span style="color: #FF6363;">Question 2.5 : </span>Calculate the Average Grade for Each Age Group

  Explanation: The groupby() function in Pandas is used to group data based on one or more columns. After grouping, you can apply aggregation functions like mean() to these groups. In this task, you will group students by their age and then calculate the average grade for each age group.

<span style="color: #ADD8E6;">_References:_</span>
- [<span style="color: #55AAFF;">W3Schools</span>](https://www.w3schools.com/python/pandas/default.asp)
- [<span style="color: #55AAFF;">Pandas Documentation</span>](https://pandas.pydata.org/docs/reference/frame.html)
- [<span style="color: #55AAFF;">GeeksforGeeks</span>](https://www.geeksforgeeks.org/pandas-tutorial/)
- [<span style="color: #55AAFF;">Pandas cheat sheet </span>](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
