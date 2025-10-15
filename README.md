# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Forward Elimination: Convert the augmented matrix to an upper triangular form by eliminating the entries below the pivot element through row operations.
2. Partial Pivoting (optional but recommended): To improve numerical stability, swap rows to position the largest absolute pivot element in the current column at the diagonal
3. Back Substitution: Solve for the variables starting from the last row upward using the upper triangular matrix
4. olution Extraction: Extract the variable values as the solution of the system.

## Program:
```
/*

Program to find the solution of a matrix using Gaussian Elimination.
Developed by:  JANANI R
RegisterNumber: 25018734
*/
```
import numpy as np
import sys
n=int(input())
a=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
  for j in range(n+1):
    a[i][j]=float(input())
for i in range(n):
  if a[i][i]==0:
    sys.exit('Divide by zero detected!')
  for j in range(i+1,n):
     ratio=a[j][i]/a[i][i]
     for k in range(n+1):
       a[j][k]=a[j][k]-ratio*a[i][k]
x[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range(n-2,-1,-1):
   x[i]=a[i][n]
   for j in range(i+1,n):
       x[i]=x[i]-a[i][j]*x[j]
   x[i]=x[i]/a[i][i]
for i in range(n):
   print('X%d = %0.2f'%(i,x[i]), end =' ')
  

    

## Output:
<img width="1120" height="591" alt="Screenshot (1)" src="https://github.com/user-attachments/assets/1b444b77-4465-4309-9791-788113275cde" />



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

