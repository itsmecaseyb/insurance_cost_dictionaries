# Python Dictionaries Medical Insurance Project

## Project Overview

This project used medical insurance data to explore the creation and use 
of Python Dictionaries.

## Methodology

Similar to the [Hurricane Analysis 
project](https://github.com/itsmecaseyb/hurricane_analysis), I used my 
existing knowledge of Python Dictionaries to complete the questions in 
this project. This project was less complex than the Hurricane Analysis 
project, and so required fewer functions and for loops to complete.

## Conclusion/Reflection

I found this project much easier to complete than the Hurricane Analysis 
project. Even so, I learned a couple of new techniques from the solution 
code.

First was the use of the `.values()` method in a for loop rather than 
indexing the dictionary, which I had been doing like so:

```
for cost in medical_costs:
    total_cost += medical_costs[cost]
```

Next was the use of multiple variables in a for loop along with the 
`.items()` method to access the key and values in the `medical_records` 
dictionary.

Question 18 asked to print a statement for each patient in the 
`medical_records` dictionary (which was a dictionary of dictionaries). In 
my code, I indexed the `medical_records` dictionary and its records like 
so:

```
for record in medical_records:
    print(record, "is a", medical_records[record]["Age"], "year old", 
medical_records[record]["Sex"], medical_records[record]["Smoker"], "with a 
BMI of", medical_records[record]["BMI"], "and insurance cost of", 
medical_records[record]["Insurance Cost"])
```

The solution code used `for name, record in medical_records.items()` and 
as a result could more easily access the values of the dictionaries within 
the `medical_records` dictionary (i.e. using `record[“Age”]` to access the 
age where I had to use `medical_records[record][“Age”]` to access the same 
information in my for loop).

Finally, I saw the solution code using backslashes (\\) to escape line 
breaks within for loops and other parts of the code to make it more 
readable, which will definitely help me make my code more readable in the 
future.
