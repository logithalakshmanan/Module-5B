# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
import pandas as pd
names=eval(input())
ages=eval(input())
designations=eval(input())

df=pd.DataFrame({
    "Name":names,
    "Age":ages,
    "Designation":designations
})
print(df)
sorted_df=df.sort_values(by="Age")
print(sorted_df)

## Output
Input	Expected	Got	
['Sanjeev', 'Keshav', 'Rahul']
[37,42,38]
['Manager', 'Clerk', 'Accountant']
      Name  Age Designation
0  Sanjeev   37     Manager
1   Keshav   42       Clerk
2    Rahul   38  Accountant
      Name  Age Designation
0  Sanjeev   37     Manager
2    Rahul   38  Accountant
1   Keshav   42       Clerk
      Name  Age Designation
0  Sanjeev   37     Manager
1   Keshav   42       Clerk
2    Rahul   38  Accountant
      Name  Age Designation
0  Sanjeev   37     Manager
2    Rahul   38  Accountant
1   Keshav   42       Clerk


## Result
**DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows is verified
