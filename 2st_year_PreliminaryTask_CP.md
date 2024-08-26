**COGNIZANCE 2<sup>st</sup> YEAR PRELIMINARY TASK**

**COMPETITIVE PROGRAMMING**

**CP AUTHORS: KAUSHIK KUMBHAT and SHYAM**

**Arrays** 
 
•	An array is a collection of data storage locations, each having the same data type and the same name. 

•	An array can be visualized as a row in a table, whose each successive block can be thought of as memory bytes containing one element. 

•	Each storage location in an array is called an array element. 

 
 
**Arrays are of two types:**

•	Single or One dimensional arrays. 

•	Multidimensional eg. two dimensional arrays. 
 
Single Dimensional Arrays 

 
•	A single dimensional array has only a single subscript. 

•	A subscript is a number in brackets that follows an array name. 

•	This number can identify the number of individual elements in the array. 

•	Individual array elements are stored in sequential memory locations. 

 ![image](https://github.com/user-attachments/assets/70a2b23d-545f-45f7-b4d8-348a002aa0b5)


1.	In this example “age” is the array of type “int” having 5 elements.
   
2.	Each element of the array is identified by the subscript number starting from 0 to 4.
   
3.	If the address of the  age[0] is 2120d and the size of int be 2 bytes,  

 
then the address of next elements shall be 

             age[1] is 2122d              
             age[2] is 2124d             
             age[3] is 2126d             
             age[4] is 2128d 
 
Accessing array elements 

•	An element is accessed by indexing the array name. 

•	This is done by placing the index of the element within square brackets after the name of the array. 

For example: 

double salary = balance[9]; 

•	The above statement will take 10th element from the array and assign the value to salary variable. 

  ![image](https://github.com/user-attachments/assets/4f357c8e-ec6d-4f09-8820-63e538960fd5)


 
•	When the above code is compiled and executed, it produces the following result: 

Element[0] = 100. 

Element[1] = 101. 

Element[2] = 102. 

Element[3] = 103. 

Element[4] = 104. 

Element[5] = 105. 

Element[6] = 106. 

Element[7] = 107. 

Element[8] = 108. 

Element[9] = 109. 


 
Example : Calculate Average 

// Program to find the average of n numbers using arrays 

 
#include <stdio.h> int main() {      

int marks[10], i, n, sum = 0, average; 

printf("Enter number of elements: ");    

scanf("%d", &n); 
 
 for(i=0; i<n; ++i) 
 
 {
 
  printf("Enter number%d: ",i+1);
 
  scanf("%d", &marks[i]); 
 
 
  // adding integers entered by the user to the sum variable
 
  sum += marks[i]; 
 
 } 
 
average = sum/n;    
  
printf("Average = %d", average); 

return 0; 
     
} 
 
 
Output 

Enter n: 5 

Enter number1: 45 

Enter number2: 35 

Enter number3: 38 

Enter number4: 31 

Enter number5: 49 

Average = 39 


Find the Largest/Smallest of the Elements of an Array 

•	We set largest to the value of the first element of the array. 

•	Then we compare this value to each of the other elements in the array. 

•	If one is larger, we replace the value in largest with the value and continue to check the rest of the array. 

 
Flow chart to find the largest of the array 
   
![image](https://github.com/user-attachments/assets/71a096de-d626-49d2-a298-19a0ea6822bb)



**TASK:**

CREATE AN ACCOUNT IN HACKERRANK PLATFORM AND JOIN IN THE HACKERRANK CHALLENGE VIA THE LINK GIVEN BELOW:

LINK: www.hackerrank.com/task-1-for-2nd-year

**SCORING CRITERIA:**

Each challenge has a pre-determined score.

A participant’s score depends on the number of test cases a participant’s code submission successfully passes.

If a participant submits more than one solution per challenge, then the participant’s score will reflect the highest score achieved. In a game challenge, the participant's score will reflect the last code submission.

Participants are ranked by score. If two or more participants achieve the same score, then the tie is broken by the total time taken to submit the last solution resulting in a higher score.
 
