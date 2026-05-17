# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required libraries (NumPy and SciPy).
2. Define the matrix using NumPy.
3. Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
4. Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
5. Display the solution and end the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Mohamed Ukkas R
RegisterNumber: 212225040245
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P, L, U = lu(matrix)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Mohamed Ukkas R
RegisterNumber: 212225040245
'''

import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu_factor, lu_solve
matrix = np.array(eval(input()))
const = np.array(eval(input()))
piv, lu = lu_factor(matrix)
ans = lu_solve((piv,lu), const)
print(ans)

```

## Output:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0db7b0e6-d020-4572-9b28-9d8cba31e40f" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/92352213-af0c-4225-9f69-da31220311ff" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

