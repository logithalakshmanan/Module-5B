# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
import pandas as pd
a=pd.DataFrame(eval(input()))
b=pd.DataFrame(eval(input()))
print('Original DataFrames:')
print(a)
print(b)
c=pd.merge(a,b,on='s_id',how='outer')
print("Merged data (outer join):")
print(c)

## Output
{'s_id': ['S1','S2','S3','S4','S5'],'name': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'],'marks': [200, 210, 190, 222, 199]}
{'s_id': ['S4', 'S5', 'S6', 'S7', 'S8'],'name': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'],'marks': [201, 200, 198, 219, 201]}
Original DataFrames:
  s_id              name  marks
0   S1  Danniella Fenton    200
1   S2      Ryder Storey    210
2   S3      Bryce Jensen    190
3   S4         Ed Bernal    222
4   S5       Kwame Morin    199
  s_id              name  marks
0   S4  Scarlette Fisher    201
1   S5  Carla Williamson    200
2   S6       Dante Morse    198
3   S7    Kaiser William    219
4   S8   Madeeha Preston    201
Merged data (outer join):
  s_id            name_x  marks_x            name_y  marks_y
0   S1  Danniella Fenton    200.0               NaN      NaN
1   S2      Ryder Storey    210.0               NaN      NaN
2   S3      Bryce Jensen    190.0               NaN      NaN
3   S4         Ed Bernal    222.0  Scarlette Fisher    201.0
4   S5       Kwame Morin    199.0  Carla Williamson    200.0
5   S6               NaN      NaN       Dante Morse    198.0
6   S7               NaN      NaN    Kaiser William    219.0
7   S8               NaN      NaN   Madeeha Preston    201.0
Original DataFrames:
  s_id              name  marks
0   S1  Danniella Fenton    200
1   S2      Ryder Storey    210
2   S3      Bryce Jensen    190
3   S4         Ed Bernal    222
4   S5       Kwame Morin    199
  s_id              name  marks
0   S4  Scarlette Fisher    201
1   S5  Carla Williamson    200
2   S6       Dante Morse    198
3   S7    Kaiser William    219
4   S8   Madeeha Preston    201
Merged data (outer join):
  s_id            name_x  marks_x            name_y  marks_y
0   S1  Danniella Fenton    200.0               NaN      NaN
1   S2      Ryder Storey    210.0               NaN      NaN
2   S3      Bryce Jensen    190.0               NaN      NaN
3   S4         Ed Bernal    222.0  Scarlette Fisher    201.0
4   S5       Kwame Morin    199.0  Carla Williamson    200.0
5   S6               NaN      NaN       Dante Morse    198.0
6   S7               NaN      NaN    Kaiser William    219.0
7   S8               NaN      NaN   Madeeha Preston    201.0


## Result
 Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame is verified
