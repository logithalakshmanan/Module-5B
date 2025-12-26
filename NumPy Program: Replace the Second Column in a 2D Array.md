# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
import pandas as pd
import ast
a=ast.literal_eval(input())
b=ast.literal_eval(input())
ser1=pd.Series(a)
print(ser1)

## Output
Input	Expected	Got	
[1, 2, 3, 4, 5]
[4, 5, 6, 7, 8]
0    1
1    2
2    3
3    4
4    5
dtype: int64
0    1
1    2
2    3
3    4
4    5
dtype: int64
[10,20,56,78,93]
[20,50,23,79,93]
0    10
1    20
2    56
3    78
4    93
dtype: int64
0    10
1    20
2    56
3    78
4    93
dtype: int64

## Result
NumPy Program: Replace the Second Column in a 2D Array is verified
