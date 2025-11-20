# NumPy Program: Row-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each row of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=1` to sort each row in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the row-wise sorted array.

## 🧾 Program
```
import numpy as np
arr=np.array(eval(input()))
print("Given array\n ",end='')
print(arr)
print()
print(np.sort(arr,axis=1))
```
## Output
![image](https://github.com/user-attachments/assets/493d2a03-fe9c-4e99-b743-474ebf0b4bd9)

## Result
Thus the *NumPy** program that sorts the elements in each row of a given 2D array in ascending order has been executed successfully.


# # 2. NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

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
```
import numpy as np
x=np.array(eval(input()))
y=np.array(eval(input()))
gt=np.where(x>y)
eq=np.where(x==y)
print(gt)
print(eq)Output
```

## Output
![5 3](https://github.com/user-attachments/assets/0e0b0671-abc1-4a9f-a978-de0052e0f504)

## Result
Thus the program that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y is executed successfully.


# NumPy Program: Program to print max from axis 0 and min from axis 1 from the given 2D Array

## 🎯 Aim
To write a python program to print max from axis 0 and min from axis 1 from the given 2-D array.

For example:
For example:

## 🧠 Algorithm
```
Step 1: Start
Step 2: Read a 2D list a from the user
Step 3: Convert the list a into a NumPy array and store it in b
Step 4: Compute the minimum element from each row of array b using np.min(b, axis=1) and store the result in c
Step 5: Compute the maximum element from each column of array b using np.max(b, axis=0) and store the result in d
Step 6: Display the original array b
Step 7: Display the row-wise minimum array c
Step 8: Display the column-wise maximum array d
Step 9: Stop
```
## 🧾 Program
```
import numpy as np
a=eval(input())
b=np.array(a)
c=np.min(a,axis=1)
d=np.max(a,axis=0)
print("Printing Original array")
print(b)
print("Printing amin Of Axis 1")
print(c)
print("Printing amax Of Axis 0")
print(d)
```

## Output
![image](https://github.com/user-attachments/assets/8c642949-6663-4a7a-8e09-f41edf64c5c9)

## Result
Thus the python program to print max from axis 0 and min from axis 1 from the given 2-D array has been executed successfully.


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
```
import pandas as pd 
import numpy as np

exam_data  = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin','Jonas'], 
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19], 
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1], 
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}

label=['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j'] 
df = pd.DataFrame(exam_data , index=label) 
print(df)
```
## Output
![5 4](https://github.com/user-attachments/assets/df3e0e5c-fef2-49d6-804c-0798da2fb50c)

## Result
Thus the program to create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows is executed successfully.


# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd
student_data1=pd.DataFrame(eval(input()))
student_data2=pd.DataFrame(eval(input()))

print("Original DataFrames:")
print(student_data1)
print("-------------------------------------")
print(student_data2)

print("\nJoin the said two dataframes along rows:")
result_data=pd.concat([student_data1, student_data2])
print(result_data)
```
## Output
![image](https://github.com/user-attachments/assets/9d4db9dc-9310-44d7-a508-804b56ce7bd6)

## Result
Thus the program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame has been executed successfully
