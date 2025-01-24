# Arithmetic Arranger

## Overview
This project was created as part of the FreeCodeCamp curriculum to complete certification requirements. It formats and arranges arithmetic problems for display, supporting addition and subtraction operations.

## Features
- Accepts up to 5 arithmetic problems at a time.
- Supports addition (`+`) and subtraction (`-`) operators.
- Validates input for errors, including:
  - Problems exceeding 5.
  - Non-digit numbers.
  - Numbers with more than four digits.
  - Unsupported operators.
- Optionally displays answers to the problems.

## Description
The **Arithmetic Arranger** is a Python program that formats and validates arithmetic problems (addition and subtraction), ensuring they meet specified constraints. It also optionally displays the answers. This project is part of the FreeCodeCamp curriculum. 🧮

## Input and Output

### Input:
The program accepts a list of arithmetic problems as strings. Each problem must be in the format:  
`<operand1> <operator> <operand2>`

For example:
```python
["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]
Output:
The program arranges the problems in a neat, readable format. If the show_answers parameter is set to True, it also displays the answers.

For example:

   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
If show_answers=True, the output includes the answers:

   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
  730      3799      88      172
