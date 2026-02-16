# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
Import the numpy module (and scipy if required) to access matrix operations and LU decomposition functions.

### Step 2:
Prepare the coefficient matrix from the given system of linear equations and store it using np.array().

### Step 3:
Apply the LU decomposition function to split the matrix into three parts:
Lower triangular matrix (L), Upper triangular matrix (U), and Permutation matrix (P).

### Step 4:
Use forward substitution to solve Ly=Pb, then backward substitution to solve Ux=y.

### Step 5:
Display the L, U (and P if used) matrices and the final solution. End the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: SARFARAZ I 
RegisterNumber: 212225230252
*/
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: SARFARAZ I 
RegisterNumber: 212225230252
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
![alt text](<Screenshot 2026-02-11 223438.png>)
![alt text](<Screenshot 2026-02-11 223508.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

