
**<span style="color: #90EE90; font-size: 1.5rem;">AI</span>**
**<span style="color: #ADD8E6; font-size: 1rem;">Authors - R. Pranav and Jagadeep</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Google Colab</span>**

**Google Colab is a free online tool that lets you write and run Python code right in your web browser. It's like a notebook where you can type your code and see the results immediately. Colab is great for learning and working on data science projects because it supports popular Python libraries like Pandas and TensorFlow. You can also use it with others, making it easy to collaborate on projects. Plus, it provides access to powerful computers (GPUs and TPUs) for faster processing, which is really helpful for running complex tasks.**

**Note: Use Google Colab to complete the tasks provided. After completing the tasks, upload your Google Colab Notebook to your GitHub repository.**

_References:_
- [<span style="color: #55AAFF;">Google Colab tutorial</span>](https://www.youtube.com/watch?v=rsBiVxzmhG0)

<hr>

**<span style="color: #FF6363; font-size: 1rem;">Question 1</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">Numpy</span>**

**NumPy is a popular Python library used for working with numbers and arrays. Think of it as a tool that helps you do math and handle large sets of numbers easily. It makes it simple to perform calculations on lists of numbers and matrices. NumPy is great for anyone who wants to do data analysis or scientific computing because it speeds up these tasks with its fast and powerful features.**

**Dataset**
**We use a dataset of details about 15 students each having attributes – Height, Weight, Age, Average Grade and Courses. We use the python code given below to create a NumPy array of our dataset.**

**Python code to create NumPy array for the task:**

---lsu

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
    
---

_Objective:_
- Design an attractive landing page for a Website/App of your own.
  (Example - Front Web Page of Amazon.com)
- The Landing page can be of your own choice, It doesn't need to be a real live Website/App.
- Make the design look as elaborate and enhanced as possible
- Make sure the design is eye-catching

_References:_
- [<span style="color: #55AAFF;">Figma Basics</span>](https://www.youtube.com/watch?v=FTFaQWZBqQ8&pp=ygUOZmlnbWEgdHV0b3JpYWw%3D)

<hr>

**<span style="color: #FF6363; font-size: 1rem;">Question 2</span>**

**<span style="color: #ADD8E6; font-size: 1rem;">RDBMS</span>**

**MySQL is a popular open-source relational database management system (RDBMS) that uses Structured Query Language (SQL) for managing and organizing data. Known for its speed, reliability, and ease of use, MySQL is widely used in web applications, data warehousing, and logging applications making it a top choice for developers and organizations to handle large volumes of data efficiently**

_Objective:_
- Download MySql from [MySql.org](https://dev.mysql.com/downloads/mysql/)
- Yet To Update

_References:_
- [<span style="color: #55AAFF;">MySQL Queries</span>](https://www.javatpoint.com/mysql-queries)
- [<span style="color: #55AAFF;">MySQL Instalation</span>](https://www.youtube.com/watch?v=u96rVINbAUI)
