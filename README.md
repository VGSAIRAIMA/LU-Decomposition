# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

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
![image]("https://github.com/VGSAIRAIMA/LU-Decomposition/blob/main/Screenshot%202026-03-22%20155048.png")
![image]("https://github.com/VGSAIRAIMA/LU-Decomposition/blob/main/Screenshot%202026-03-22%20155101.png")


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

