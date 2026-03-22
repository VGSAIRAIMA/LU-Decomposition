# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm


1. **Input** the order ( n ) and elements of the square matrix ( A ).

2. **Initialize** matrix ( L ) as an identity matrix and matrix ( U ) as a zero matrix.

3. **Compute** the elements of ( L ) and ( U ) using LU decomposition formulas until all rows and columns are completed.

4. **Display** matrices ( L ) and ( U ) such that ( A = LU ) and stop the program.



## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: V G SAIRAIMA
RegisterNumber: 212225040359
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: V G SAIRAIMA
RegisterNumber: 212225040359
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
b=np.array(eval(input()))
P,L,U=lu(a)
y=np.linalg.solve(L,P@b)
x=np.linalg.solve(U,y)
print(x)
```

## Output:
![alt text](<Screenshot 2026-03-22 155048.png>)
![image](https://github.com/VGSAIRAIMA/LU-Decomposition/blob/main/Screenshot%202026-03-22%20155101.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

