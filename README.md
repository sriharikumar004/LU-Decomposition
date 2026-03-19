# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required Python libraries NumPy and SciPy.

2.Read the input matrix (and constant matrix for equations) from the user

3.Perform LU Decomposition using the built-in SciPy functions to obtain L and U matrices.

4.Display the L matrix, U matrix, and the solution of the system of equations, then stop the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: sriharikumar k 
RegisterNumber:212225230273
'''
import numpy as np
from scipy .linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: sriharikumar k
RegisterNumber: 212225230273
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:
<img width="909" height="955" alt="Screenshot 2026-03-18 145740" src="https://github.com/user-attachments/assets/fbfc3608-d215-417d-b881-99bf21f0e0f1" />

<img width="900" height="862" alt="Screenshot 2026-03-18 145804" src="https://github.com/user-attachments/assets/bfd768a7-e2fd-4459-9c05-671526b847b1" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

