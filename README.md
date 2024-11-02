# Student Name: [Bin Ware](https://github.com/bware7/python-ds-nb-binware)

# Python Data Structures and Notebooks

## Project Summary
This project covers fundamental concepts in Python programming, focusing on data structures, basic operations, and Jupyter notebooks. The tasks include implementing mathematical operations, writing custom functions, working with dictionaries and lists, and building a pattern-drawing program in Python. The project demonstrates key skills in using Python for data analysis, iteration, and managing collections, as well as documenting work effectively.

## Rubric
Each question is worth one point.

# Task 1: Division Code
```python
def divide_numbers(a, b):
    result = a / b
    print(f"Division result: {result}")

divide_numbers(10, 2)
```

# Task 2: Factorial of Integers from 1 to 10
```python
for i in range(1, 11):
    factorial = 1
    for j in range(1, i + 1):
        factorial *= j
    print(f"Factorial of {i}: {factorial}")
```

# Task 3: Mean Function
```python
def calculate_mean(values):
    return sum(values) / len(values)

testlist = [1, -1, 2, -2, 3, -3, 4, -4]
mean_value = calculate_mean(testlist)
print(f"Mean of testlist: {mean_value}")
```

# Task 4: Variance Function
```python
def calculate_variance(values):
    mean = calculate_mean(values)
    squared_diffs = [(x - mean) ** 2 for x in values]
    variance = sum(squared_diffs) / len(values)
    return variance

list1 = [5.670e-1, -1.480e+0, -5.570e-1, -1.470e+0, 7.340e-1, 1.050e+0, 4.480e-1, 2.570e-1, -1.970e+0, -1.460e+0]
list2 = [-1.780e+0, 2.640e-1, 1.160e+0, 9.080e-1, 1.780e+0, 1.080e+0, 1.050e+0, -4.630e-2, 1.520e+0, 5.350e-1]

variance_list1 = calculate_variance(list1)
variance_list2 = calculate_variance(list2)
print(f"Variance of list1: {variance_list1}")
print(f"Variance of list2: {variance_list2}")
```

# Task 5: List Slicing
```python
my_list = [i for i in range(1, 21)]
print("First 5 elements:", my_list[:5])
print("Last 5 elements:", my_list[-5:])
print("List reversed:", my_list[::-1])
print("Every second element:", my_list[::2])
print("Every third element:", my_list[::3])
```

# Task 6: Dictionary of Class Information
```python
class_info = {
    "name": "Web Mining and Applied NLP",
    "course_number": "44-620",
    "semester": "Fall 2024",
    "credit_hours": 3,
    "learning_objectives": [
        "Understand web mining techniques",
        "Apply natural language processing",
        "Analyze and interpret web data",
        "Develop data-driven web applications"
    ]
}
print("Class Information:", class_info)
```

# Task 7: Print Level 3 Spells
```python
player_character = {
    'name': 'Kitab',
    'class': [('Cleric: Knowledge', 7)],
    'spells': {
        'cantrip': ['Guidance', 'Light', 'Thaumaturgy', 'Toll the Dead', 'Word of Radiance'],
        'level 1': ['Command', 'Detect Magic', 'Healing Word', 'Identify', 'Sleep'],
        'level 2': ['Augury', 'Calm Emotions', 'Command', 'Invisibility', 'Lesser Restoration'],
        'level 3': ['Mass Healing Word', 'Nondetection', 'Revivify', 'Feign Death', 'Speak with Dead'],
        'level 4': ['Banishment', 'Confusion']
    }
}
print("Level 3 Spells:", player_character['spells']['level 3'])
```

# Task 8: Unique Elements in List
```python
values = [10, 11, 10, 8, 1, 12, 0, 1, 6, 5, 5, 13, 6, 15, 0, 0, 1, 1, 9, 7]
unique_values = set(values)
print(f"Number of unique elements: {len(unique_values)}")
```

# Task 9: Create a New Jupyter Notebook
Note: Create a Jupyter notebook named "s577829.ipynb" with the pattern code below.

## Pattern Drawing Code
```python
for i in range(1, 5):
    stars = '*' * i
    spaces = ' ' * (8 - 2 * i)
    print(stars + spaces + stars)
```

Output:
```
*      *
**    **
***  ***
********
```
