# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : Import the numpy module to use the built_in functions for calculation
### Step 2: Prepare the lists from the matrix and assign in np.array()
### Step 3: using the np.linalg.inv(), we can find the solutions.
### Step 4: End the program

## Program:

```
import numpy as np

def find_matrix_inverse(matrix):

    try:
        np_matrix = np.array(matrix)
        inverse = np.linalg.inv(np_matrix)
        return inverse
    except np.linalg.LinAlgError:
        return None 
    except Exception as e:
        print(f"An error occurred: {e}")
        return None

matrix = [[2, 1, 1],
          [1, 1, 1],
          [1, -1, 2]]

inverse = find_matrix_inverse(matrix)

if inverse is not None:

    print(inverse)
else:
    print("The matrix is singular (non-invertible).")
```
## output:
![Screenshot 2025-03-27 201101](https://github.com/user-attachments/assets/4a74f8ef-ca21-49f1-a894-fba330fe1a64)



## Result:
Thus the inverse of given matrix is successfully solved using python program

