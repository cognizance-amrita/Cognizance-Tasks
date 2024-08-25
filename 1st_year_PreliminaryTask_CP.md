<b>COGNIZANCE 1<sup>st</sup>  YEAR PRELIMINARY TASK</b> 

**COMPETITIVE PROGRAMMING**

1. **BASIC IUPUT AND OUTPUT:**

In programming, **input** and **output** are fundamental concepts that allow a program to interact with its environment, typically by receiving data from the user (input) and presenting results or information (output).

**A simple example of python code involving both user input and output:**

#Simple calculator

num1 = float(input("Enter the first number: "))

num2 = float(input("Enter the second number: "))

operation = input("Enter an operation (+, -, \*, /): ")

if operation == "+":

`    `result = num1 + num2

elif operation == "-":

`    `result = num1 - num2

elif operation == "\*":

`    `result = num1 \* num2

elif operation == "/":

`    `result = num1 / num2

else:

`    `result = "Invalid operation"

print(f"The result is: {result}")

1. **CONDITIONAL STATEMENTS:**

Conditional statements are a fundamental concept in programming that allows you to make decisions based on certain conditions. These statements enable your code to execute different blocks of code depending on whether specific conditions are met or not. In this blog post, we'll delve into the basics of conditional statements, starting with the ubiquitous if-else statement and gradually exploring more complex scenarios.

**A SIMPLE FLOWCHART DEMONSTRATING THE WORKING OF CONDITIONAL STATEMENT IS SHOWN AS BELOW:**

![](Aspose.Words.f4a401df-219a-4aa5-b491-299bdda83a47.001.png)

- 'if statement' is used to execute a block of code only if a certain condition is met. It allows us to conditionally execute code based on whether the specified condition is true.

- 'else statement', on the other hand, is an optional companion to the if statement. It specifies what code to execute if the condition in the if statement is not met (i.e. if it is false).

1. **INTRODUCTION TO FOR LOOP:**

A for loop is a control structure in programming that allows you to execute a specific block of code repeatedly. It's especially useful when you want to perform the same task multiple times without duplicating your code. Let's break down the essential components of a for loop:

`
`**1.  Initialization:** You declare and initialize a variable that serves as a counter. This step only happens once at the beginning.

2. **Condition:** You specify a condition that determines when the loop should stop executing.
Increment/Decrement: You define how the counter variable changes after each iteration.

![](Aspose.Words.f4a401df-219a-4aa5-b491-299bdda83a47.002.png)

![](Aspose.Words.f4a401df-219a-4aa5-b491-299bdda83a47.003.png)

2. **INTRODUCTION TO WHILE LOOP:**

A while loop follows a simple sequence of steps:

**1. Evaluation of Test Expression:** The loop begins by evaluating a test expression.
Condition Check: If the test expression is true, the code inside the loop's body is executed.


**2. Re-evaluation:** After executing the code, the test expression is evaluated again.
Continuation or Termination: This process continues until the test expression becomes false, at which point the while loop terminates.

![](Aspose.Words.f4a401df-219a-4aa5-b491-299bdda83a47.004.png)

While loops can be best illustrated with the practical example of finding the Factorial. Factorial of a number 'n' is the product of all positive integers from 1 to 'n'. To compute this using a while loop, we initialise a factorial variable to 1 and repeatedly multiply it by 'n' while decrementing 'n' until 'n' becomes 0. This ensures that we calculate the factorial correctly.

**5. INTROUCTION TO FUNCTIONS:**

In programming, a **function** is a block of code designed to perform a specific task. Functions help organize code, make it reusable, and improve its readability. Instead of writing the same code multiple times, you can define a function once and call it whenever you need it.

**Why to use Functions?**

- **Reusability:** Write a function once, use it many times.

- **Organization:** Break down complex problems into smaller, manageable parts.

- **Modularity:** Functions allow you to organize code into separate sections.

- **Maintainability:** Easier to update code. Changes in a function are reflected wherever the function is used.

Tasks for Week 1:


