# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
## 3. Implementation of programs using conditional statements.
## 4. Implementation of programs using various control statements.
# Ex.No:6
  Build a C program to input a student’s marks in three subjects (Math, Science, and English). Calculate the average marks and determine the grade using nested if-else statements with safe floating-point comparisons based on the following grading criteria:
    
  A: 90 and above
  
  B: 75 to 89.99
  
  C: 50 to 74.99
  
  F: below 50
  
  The program should display the average marks up to two decimal places and the corresponding grade. 
  
# Date : 
# Aim:
 To build a C program that receives inputs for a student’s marks in three subjects, calculates the average, and determines the grade using nested if-else statements with safe floating-point comparisons.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare float variables math, science, english to store marks of each subject.
### Step 4: 
  Declare a float variable average to store the average marks.
### Step 5: 
  Prompt the user to enter marks for Math, Science, and English.
### Step 6: 
  Read the input marks.
### Step 7: 
  Calculate the average marks using the formula:
   
  average=(math + science + english​)/3.0f
### Step 8: 
  Check if average is greater than or equal to 90.0f

  If yes, print Grade A.

  Else, proceed to Step 9.  
### Step 9:
  Check if average is greater than or equal to 75.0f

  If yes, print Grade B.

  Else, proceed to Step 10.
### Step 10:
  Check if average is greater than or equal to 50.0f

  If yes, print Grade C.

  Else, print Grade F.
### Step 11:
  Stop
# Program:
```
#include <stdio.h>

int main() { float math, science, english; float average;

// Input marks
printf("Enter marks for Math: ");
scanf("%f", &math);

printf("Enter marks for Science: ");
scanf("%f", &science);

printf("Enter marks for English: ");
scanf("%f", &english);

// Calculate average
average = (math + science + english) / 3.0;

// Display average
printf("\nAverage Marks = %.2f\n", average);

// Determine grade using nested if-else
if (average >= 90.0) {
    printf("Grade: A\n");
} 
else {
    if (average >= 75.0) {
        printf("Grade: B\n");
    } 
    else {
        if (average >= 50.0) {
            printf("Grade: C\n");
        } 
        else {
            printf("Grade: F\n");
        }
    }
}

return 0;
```
# Output:
<img width="441" height="242" alt="image" src="https://github.com/user-attachments/assets/210c5364-d595-467a-9d73-780d91949fe7" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:7
  Develop a C program to display the multiplication table of a given number (15) up to 10.
# Date : 
# Aim:
 To develop a C program that prints the multiplication table of the number 15 up to 10 using a for loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare an integer variable number and initialize it with 15.
### Step 4: 
  Declare another integer variable i to use as a loop counter.
### Step 5: 
  Use a for loop to iterate from i = 1 to i = 10.
  
  In each iteration:
  
  a. Multiply number by i.
  
  b. Print the result in the format: number x i = result.
### Step 6: 
  Stop

# Program:
```
#include <stdio.h>

int main() { int num = 15;

printf("Multiplication Table of %d:\n\n", num);

for (int i = 1; i <= 10; i++) {
    printf("%d x %d = %d\n", num, i, num * i);
}

return 0;
```
# Output:
<img width="541" height="402" alt="image" src="https://github.com/user-attachments/assets/0dc6890d-0bb6-4563-97bb-d1310f115eac" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:8
  Develop a C program to check whether a given number is prime or not.
# Date : 
# Aim:
 To develop a C program that determines whether an input number is a prime number using a while loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables:
  
  n to store the number entered by the user.
  
  i to use as a counter (initialize to 2).
  
  f as a flag to indicate whether the number is divisible (initialize to 0).
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Use a while loop to iterate while i <= n-1:
  
  Check if n % i == 0:

  If yes, set f = 1 (number is not prime) and break the loop.
  
  Increment i by 1.
### Step 6: 
  After the loop:
  
  If f == 0, print that the number is prime.
  
  Else, print that the number is not prime.
### Step 7:   
  Stop
# Program:
```
#include <stdio.h>

int main() { int num, i, isPrime = 1;

// Input number
printf("Enter a number: ");
scanf("%d", &num);

// Numbers less than or equal to 1 are not prime
if (num <= 1) {
    isPrime = 0;
} 
else {
    // Check divisibility from 2 to num/2
    for (i = 2; i <= num / 2; i++) {
        if (num % i == 0) {
            isPrime = 0;
            break;
        }
    }
}

// Output result
if (isPrime)
    printf("%d is a Prime number.\n", num);
else
    printf("%d is NOT a Prime number.\n", num);

return 0;
```
# Output:
<img width="468" height="152" alt="image" src="https://github.com/user-attachments/assets/80d7abc5-849d-41a4-9c65-48dbef064976" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:9
  Generate the C code to display the pattern below.  
 ``` 
 12345  
 2   4  
 3   3  
 4   2  
 54321
 ```
# Date : 
# Aim:
 To build a C program that prints the required numeric pattern for a given value of n using nested loops.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare variables i, j, n, and k.
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Set i = 1.
### Step 6:  
  Repeat the following steps until i > n:
  
  Step 6.1: For j from i to n, print j if i == 1 or j == i, otherwise print a space.
  
  Step 6.2: Set k = j - 2.
  
  Step 6.3: For j from 1 to i - 1, print k if i == n or j == i - 1, otherwise print a space.
  
  Step 6.4: Decrease k after each print.
  
  Step 6.5: Move to the next line.
  
### Step 7: 
  Increase i and repeat Step 6.
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() { int i, j;

// First row
for (j = 1; j <= 5; j++) {
    printf("%d", j);
}
printf("\n");

// Middle rows
for (i = 2; i <= 4; i++) {
    for (j = 1; j <= 5; j++) {
        if (j == 1)
            printf("%d", i);
        else if (j == 5)
            printf("%d", 6 - i);
        else
            printf(" ");
    }
    printf("\n");
}

// Last row
for (j = 5; j >= 1; j--) {
    printf("%d", j);
}

return 0;
```
# Output:
<img width="181" height="210" alt="image" src="https://github.com/user-attachments/assets/faa045dd-c664-4e74-b3b3-1f7573d597a7" />

# Result: 
  Thus, the program was implemented and executed successfully, and the required output was obtained.

  
# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:10
  Generate the C code to display the pattern below.  
  
 0
 
 7  0  7
 
 6  7  0  7  6
 
 5  6  7  0  7  6  5
 
 4  5  6  7  0  7  6  5  4
 
 3  4  5  6  7  0  7  6  5  4  3
 
 2  3  4  5  6  7  0  7  6  5  4  3  2
 
 1  2  3  4  5  6  7  0  7  6  5  4  3  2  1

# Aim: 
  To formulate a C program to print a symmetric numeric pattern in which each row contains an increasing sequence of numbers from the row value up to 7, followed by 0 in the center, and then a decreasing sequence of numbers back to the row value.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables i and j.
### Step 4: 
  Print 0 on the first line.
### Step 5:
  Set i = 7.
### Step 6:
   Repeat Steps 6.1 to 6.4 while `i >= 1`:

   Step 6.1: For `j = i` to `7`, print `j`.

   Step 6.2: Print `0` in the center.

   Step 6.3: For `j = 7` down to `i`, print `j`.

   Step 6.4: Move to the next line.
### Step 7:
  Decrease i by 1 and go back to Step 6.
### Step 8:
  Stop
### Program:
```
#include <stdio.h>

int main() { int i, j;

// First row
for (j = 1; j <= 5; j++) {
    printf("%d", j);
}
printf("\n");

// Middle rows
for (i = 2; i <= 4; i++) {
    for (j = 1; j <= 5; j++) {
        if (j == 1)
            printf("%d", i);
        else if (j == 5)
            printf("%d", 6 - i);
        else
            printf(" ");
    }
    printf("\n");
}

// Last row
for (j = 5; j >= 1; j--) {
    printf("%d", j);
}

return 0;
```
###Output:
<img width="401" height="310" alt="image" src="https://github.com/user-attachments/assets/8ab45a05-8e92-45f3-b75f-7a3b1cd7c63b" />

# Result:
  Thus, the program was implemented and executed successfully, and the required output was obtained.

