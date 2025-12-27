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
~~~
import pandas as pd 

student_data1 = pd.DataFrame({ 
'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'], 

'name': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'],  

'marks': [200, 210, 190, 222, 199]}) 

student_data2 = pd.DataFrame({ 
'student_id': ['S4', 'S5', 'S6', 'S7', 'S8'], 

'name': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'], 

'marks': [201, 200, 198, 219, 201]}) 

print("Original DataFrames:") 

print(student_data1)

print("-------------------------------------") 

print(student_data2) 

print("\nJoin the said two dataframes along rows:") 

result_data = pd.concat([student_data1, student_data2]) 

print(result_data)
~~~
## Output
<img width="713" height="909" alt="530385999-b75da311-acc8-4a7f-8d4d-d03f6c1ffbec" src="https://github.com/user-attachments/assets/48caef18-4db6-4123-b179-29e5f2e2463d" />

## Result
Thus, the Python program has been successfully created and executed successfully to join the two DataFrames row-wise using pd.concat() and all records from both DataFrames were included in the final output .
