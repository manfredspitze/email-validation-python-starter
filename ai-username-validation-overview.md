A basic activity that will teach you how to use both the `isalpha()` and `isdigit()` string methods to validate string input.

---

### Task: Validate a Username

**Description:**

The task is to write a Python script that validates a username based on the following rules:

1. **Part 1**: The script should first check if the username consists only of letters (no numbers or special characters). This can be done using the `isalpha()` method.
   
2. **Part 2**: The script should then check if the username is a valid number (i.e., it consists only of digits). This can be done using the `isdigit()` method.

After completing both checks, the program should:
- If the username consists only of letters, print `"Username is valid (consists of letters only)!"`.
- If the username consists only of digits, print `"Username is valid (consists of digits only)!"`.
- If the username fails both checks, print `"Invalid username!"`.

### Requirements:

- Use `isalpha()` to check for letters only in Part 1.
- Use `isdigit()` to check for digits only in Part 2.
  
---

### Example:

**Input 1:**
```
Enter your username: Alice
```
**Output 1:**
```
Username is valid (letters only)!
```

**Input 2:**
```
Enter your username: 123456
```
**Output 2:**
```
Username is valid (digits only)!
```

**Input 3:**
```
Enter your username: Alice123
```
**Output 3:**
```
Invalid username!
```

---

### Script Hints:

```python
# Function takes just one parameter -- `username`
def validate_username(parameter):
    # Use `isalpha ( )` method to check if the username consists only of alphabetic characters (letters)
    if condition:
        return "Username is valid (letters only)!"
    # Part 2: Check if the username consists only of digits
    elif condition:
        return "Username is valid (digits only)!"
    else:
        return "Invalid username!"

# Prompt user for a username

# Call function to validate username and print message about username
print( )
```

### Explanation:
- **Part 1 (`isalpha()`):** This method returns `True` if all characters in the string are alphabetic (i.e., they are letters). It will return `False` if there are any numbers or special characters.
- **Part 2 (`isdigit()`):** This method returns `True` if all characters in the string are digits (i.e., numbers). It will return `False` if there are any alphabetic characters or special symbols.

### How to Approach Validating The Username:
1. **Input validation**: First, write the code that checks if the input consists only of alphabetic characters using `isalpha()`.
2. **Second check**: Then, check if the input consists only of digits using `isdigit()`.
3. **Conditionals**: Use `if-elif-else` statements to let users know whether their input meets the requirements.

### Example of Valid Inputs:
- `"Alice"` (valid, all letters)
- `"123456"` (valid, all digits)
- `"Alice123"` (invalid, contains both letters and digits)

