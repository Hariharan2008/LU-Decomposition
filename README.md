# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Import the numpy module to use the built-in functions for calculation

Step 2: Prepare the lists from each linear equations and assign in np.array()

Step 3: Using scipy.linalg import lu ,we can find L and U matix.

Step 4: By using lu_factor ,lu_solve .we can find lu decomposition matrix.

Step 5: End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: S.HARIHARAN
RegisterNumber: 212225040109
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: S.HARIHARAN
RegisterNumber: 212225040109
'''
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=[[3, 2, 7], [2, 3, 1], [3, 4, 1]] 
b=[4, 5, 7] 
piv,lu=lu_factor(a)
result=lu_solve((piv,lu),b)
print(result)
```

## Output:

<img width="1217" height="992" alt="Screenshot 2026-05-20 094621" src="https://github.com/user-attachments/assets/c9d52977-a5dd-4ce5-b4bb-23b421e50eda" />

<img width="1432" height="1017" alt="Screenshot 2026-05-20 094639" src="https://github.com/user-attachments/assets/7a23f784-0e1b-4244-9dcf-357031c25b9e" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

