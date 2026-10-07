# PLP Python Week 6 - Safe Functions

## File Descriptions
* `safe_tools.py`: Contains functions using try-except blocks to handle division, string conversion, and dictionary lookups safely without crashing.

## Reflection Question
### Why can an `if` check not catch "abc" on its own?
An `if` statement checks whether a condition evaluates to true or false, but checking if an arbitrary string can be converted to an integer (such as handling negative numbers, leading/trailing whitespaces, or non-digit characters) requires parsing logic. In Python, `int("abc")` raises a `ValueError` at runtime during the type conversion, which cannot be prevented simply by testing string existence without attempting the conversion itself or using exception handling.
