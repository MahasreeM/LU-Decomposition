# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy and scipy module to use the built-in functions for calculation
2. Prepare the lists for the given matrix and assign in np.array()
3. Using the scipy.linalg.lu(),we get L AND U of the given matrix. Using the scipy.linalg.lu_factor()
and scipy.linalg.lu_solve we get the LU decomposition of the given matrix.
4. End of the program

## Program:

'''Program to find L and U matrix using LU decomposition.
Developed by: Maha shree.M
RegisterNumber: 24900438
'''

(i) To find the L and U matrix

    import numpy as np
    from scipy.linalg import lu
    A=np.array(eval(input()))
    P,L,U=lu(A)
    print(L)
    print(U)


(ii) To find the LU Decomposition of a matrix

    import numpy as np
    from scipy.linalg import lu_factor,lu_solve
    A=np.array(eval(input()))
    b=np.array(eval(input()))
    lu,piv=lu_factor(A)
    x=lu_solve((lu,piv),b)
    print(x)


## Output:
![lu decomposition]()
![alt text](<Screenshot (74).png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

