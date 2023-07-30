# LU Decomposition 

## AIM:
### (i) To find the L and U matrix
To write a program to find the LU of a matrix.
### (ii) To find the LU Decomposition of a matrix
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrix
1. Import numpy library using import statement.
2. From scipy package import lu().
3. Get input from user and pass it as an array
4. Get P, L, U matrix using lu()
5. Print L and U matrix

### (ii) To find the LU Decomposition of a matrix
1. Import numpy library using import statement
2. From scipy package import lu_factor() and lu_solve().
3. Get two inputs from user and pass it as matrix array.
4. Find lu and pivot value of first matrix using lu_factor()
5. Find solution of the matrix by using lu_solve() by passing lu, pivot values as first argument and second matrix as second argument
6. Print the solution.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Abishai K C   
RegisterNumber: 23001564    
'''
from scipy.linalg import lu
a = eval(input())
P,L,U = lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Abishai K C
RegisterNumber: 23001564
'''

# To print X matrix (solution to the equations)
from scipy.linalg import lu_factor,lu_solve
a = eval(input())
b = eval(input())
lu,piv = lu_factor(a)
x = lu_solve((lu,piv),b)
print(x)
```

## Output:

### L and U matrix
![lu decomposition](/lu%20-1%20.png)

### LU Decomposition of a matrix
![output](/lu%20-2.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

