# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start
2. Input the coefficient matrix A.
3. Input the constant matrix (right-hand side vector) B.
4. Perform LU factorization of matrix A using lu_factor(A), which returns: A combined matrix containing the factors of L and U. A pivoting array P representing row interchanges.
5.Solve the system of equations AX=B using the LU factors and the pivoting array with lu_solve((L, P), B).
6. Store the result in variable X.
7. Print the solution vector X.
8. End
## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: DHARSHAN R
RegisterNumber: 212224230060
*/
import numpy as np
from scipy.linalg import lu

a = np.array(eval(input()))
p,l,u = lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: DHARSHAN R
RegisterNumber: 212224230060
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve

A = np.array(eval(input()))
B = np.array(eval(input()))

L,P=lu_factor(A)
X = lu_solve((L,P),B)

print(X)
```

## Output:
<img width="817" height="836" alt="Screenshot 2026-03-10 213011" src="https://github.com/user-attachments/assets/ab636ee9-39ff-404b-a5f2-17b1d8e5df04" />

<img width="774" height="296" alt="Screenshot 2026-03-10 213034" src="https://github.com/user-attachments/assets/dc38e438-0fa8-425a-9214-f697159e3e1a" />

<img width="871" height="946" alt="Screenshot 2026-03-10 213729" src="https://github.com/user-attachments/assets/0551a03f-ca90-4d74-ae02-eb7e61269b4c" />


<img width="585" height="127" alt="Screenshot 2026-03-10 213053" src="https://github.com/user-attachments/assets/1ec229b9-fb90-410b-b2c2-d853ea564f08" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

