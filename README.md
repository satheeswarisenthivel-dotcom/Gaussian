# Exp-6 Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read number of unknowns n.
   Read augmented matrix A[n][n+1].
2.For i = 0 to n-1
  If A[i][i] == 0, stop (division by zero).
  For j = i+1 to n-1
  Find ratio = A[j][i] / A[i][i]
  For k = 0 to n
  A[j][k] = A[j][k] - ratio * A[i][k] 
3.Back Substitution
  x[n-1] = A[n-1][n] / A[n-1][n-1]
  For i = n-2 to 0
   x[i] = A[i][n]
   For j = i+1 to n-1
   x[i] = x[i] - A[i][j] * x[j]
    x[i] = x[i] / A[i][i] 
4. Print the solution vector x[i].
## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: SATHEESWARI.S
RegisterNumber: 212225240141
*/
```

## Output:
<img width="616" height="881" alt="567272535-dfccd644-d10a-4810-948f-951ddcc28f06" src="https://github.com/user-attachments/assets/0450eddf-f772-4d4f-88e4-661137589050" />

<img width="458" height="193" alt="image" src="https://github.com/user-attachments/assets/c47133ae-d073-43b7-a3bc-8419733e6a8a" />

## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

