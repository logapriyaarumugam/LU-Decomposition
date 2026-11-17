# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program.
2. Import the required NumPy and SciPy libraries and get the matrix as input.
3. Using the LU decomposition method, we can decompose the given matrix into Lower and Upper triangular matrices.
4. Display the Lower and Upper triangular matrices and stop the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Logapriya A
RegisterNumber: 212225040202
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
Developed by: Logapriya A
RegisterNumber: 212225040202
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
<img width="835" height="452" alt="image" src="https://github.com/user-attachments/assets/e9e31ba8-0bf3-49e2-a17d-6ba18200c387" />
<img width="850" height="317" alt="image" src="https://github.com/user-attachments/assets/b13999e3-4c2f-4a4d-a86c-396a4b9eb80b" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

