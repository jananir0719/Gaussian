# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import NumPy.
Take the augmented matrix as a NumPy array (combine coefficients and constants).
2. For each pivot row i:
Find the pivot element A[i][i].
Make the pivot element 1 (divide the entire row by the pivot).
Eliminate all entries below the pivot (make them zero using row operations).
3. Start from the last row and move upward.
  Eliminate entries above the pivots to make zeros.
4. The last column of the matrix now contains the solutions.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: JANANI R
RegisterNumber: 25018734
*/
```
<img width="920" height="702" alt="Screenshot 2025-10-11 150748" src="https://github.com/user-attachments/assets/eb315659-e81f-494e-b08e-fc13de87f948" />


## Output:<img width="782" height="571" alt="Screenshot 2025-10-11 150805" src="https://github.com/user-attachments/assets/db4753cf-6746-4a7b-a1f5-8e019ac6104a" />



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

