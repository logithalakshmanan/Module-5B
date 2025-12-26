# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
import numpy as np
N,M,P=map(int,input().split())
arr1=np.array([list(map(int,input().split())) for _ in range(N)])
arr2=np.array([list(map(int,input().split())) for _ in range(M)])
result=np.concatenate((arr1,arr2),axis=0)
print(result)

## Output
	Input	Expected	Got	
    4 3 2
    1 2
    1 2
    1 2
    1 2
    3 4
    3 4
    3 4
[[1 2]
 [1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]
 [3 4]]
[[1 2]
 [1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]
 [3 4]]
    3 3 2
    1 2
    1 2
    1 2
    3 4
    3 4
    3 4
[[1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]
 [3 4]]
[[1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]
 [3 4]]
    3 2 2
    1 2
    1 2
    1 2
    3 4
    3 4
[[1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]]
[[1 2]
 [1 2]
 [1 2]
 [3 4]
 [3 4]]


## Result
 NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y is verified
