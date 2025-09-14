# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
~~~
1.Import the numpy module and lu module from scipy.linalg to use the built-in functions for calculation
2.Prepare the lists from each linear equations and assign in np.array()
3.Using the lu(), we get three results (first is P, second is L and third is U) of the given matrix.
4.Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable.
5.End the program
~~~

(ii):
~~~
1.Start
2.Input the matrix A and vector b
3.Use LU Decomposition to factor the matrix A into L (lower triangular) and U (upper triangular) → Use lu_factor(A)
4.Solve the equation Ax = b using the LU factors → Use lu_solve((lu, piv), b)
5.Print the solution vector x
6.End
~~~

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)


```
(ii) To find the LU Decomposition of a matrix
```
import numpy as np
from scipy.linalg import lu_factor, lu_solve
a = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(a)
x = lu_solve((lu, piv), b)
print(x)

```

## Output:

<img width="1873" height="1023" alt="image" src="https://github.com/user-attachments/assets/72a6ad09-8d62-4185-ae56-09d416611908" />
<img width="1860" height="943" alt="image" src="https://github.com/user-attachments/assets/30ce1ef8-c889-4f42-b97c-d902a034761e" />

<img width="1834" height="964" alt="image" src="https://github.com/user-attachments/assets/df105ed7-fdda-4aa5-87db-4e17205389b6" />
<img width="1862" height="994" alt="image" src="https://github.com/user-attachments/assets/1f178b7e-1ef5-45ef-8a9b-c51b0f1c0448" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

