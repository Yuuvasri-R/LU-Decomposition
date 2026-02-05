# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Yuuvasri R
RegisterNumber: 212225230313
'''
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
Developed by: Yuuvasri R
RegisterNumber: 212225230313
'''
# To print X matrix (solution to the equations)
import numpy as np

from scipy.linalg import lu_factor,lu_solve

A=np.array(eval(input()))

B=np.array(eval(input()))

lu,pivot=lu_factor(A)

x=lu_solve((lu,pivot),B)

print(x)
```

## Output:
<img width="1252" height="491" alt="Screenshot 2026-02-05 142645" src="https://github.com/user-attachments/assets/801ee50d-5cc8-4f50-9516-6f7e55674e28" />
<img width="1071" height="322" alt="Screenshot 2026-02-05 142659" src="https://github.com/user-attachments/assets/0a53c622-b449-4669-a44c-05ca992620fd" />


## Result:

Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.





