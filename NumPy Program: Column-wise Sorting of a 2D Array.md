# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
Add code hereimport numpy as np
arr=np.array(eval(input()))
print("The original array:")
print(f" {arr}")

arr_2d=arr.reshape(3,3)
print("\n3 x 3 Array:")
print(f" {arr_2d}")
## Output
Input	Expected	Got	
 [0, 1, 2, 3, 4, 5, 6, 7, 8]
The original array:
[0 1 2 3 4 5 6 7 8]
The original array:
 [0 1 2 3 4 5 6 7 8]

3 x 3 Array:
 [[0 1 2]
 [3 4 5]
 [6 7 8]]
The original array:
 [0 1 2 3 4 5 6 7 8]

3 x 3 Array:
 [[0 1 2]
 [3 4 5]
 [6 7 8]]
[11, 12, 13, 14, 15, 16, 17, 18, 19]
The original array:
 [11 12 13 14 15 16 17 18 19]

3 x 3 Array:
 [[11 12 13]
 [14 15 16]
 [17 18 19]]
The original array:
 [11 12 13 14 15 16 17 18 19]

3 x 3 Array:
 [[11 12 13]
 [14 15 16]
 [17 18 19]]

## Result
NumPy program that sorts the elements in each column of a given 2D array in ascending order is verified
