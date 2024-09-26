# Roman Numeral Converter

## Description

This Python script converts an integer to its corresponding Roman numeral representation. It works with both positive and negative integers. For negative numbers, it converts the absolute value of the number into a Roman numeral, while for `0`, it prints "Not Applicable" since Roman numerals do not have a representation for zero.

## Features

- Converts positive integers to Roman numerals.
- Handles negative integers by converting the absolute value and displaying a custom message.
- Prompts user input repeatedly until the script is terminated manually.
- Prints "Not Applicable" for zero.

## How It Works

1. **Function `int_to_roman(num)`**:
   - This function takes an integer `num` as input and converts it into a Roman numeral.
   - The function uses a dictionary of Roman numeral symbols, mapping them to corresponding integer values.
   - It iterates through the dictionary in descending order, subtracting the largest possible Roman numeral value from the input number and appending the corresponding Roman numeral to the result string until the input number becomes zero.

2. **Main Loop**:
   - The script continuously asks for a user input using `input()`.
   - If the number is zero, it prints "Not Applicable."
   - If the number is negative, it calculates the Roman numeral of its absolute value and displays a message indicating that Roman numerals are not applicable to negative numbers.
   - If the number is positive, it directly converts the number to Roman numerals and prints the result.

## Example

```bash
Enter number: 23
The Roman numeral for 23 is: XXIII

Enter number: 0
Not Applicable

Enter number: -7
The Roman numeral for -7 is not applicable. However, the Roman numeral for its absolute value is: VII
```

## Requirements

- Python 3.x

## How to Run

1. Copy the code into a Python file (e.g., `roman_numeral_converter.py`).
2. Run the script in a terminal or command prompt:

   ```bash
   python3 roman_numeral_converter.py
   ```

3. Enter a number when prompted, and the script will display the Roman numeral equivalent.

## Limitations

- The script handles only integers. If non-integer input is given, it will raise an error.
- It does not handle large numbers beyond the range typically represented by Roman numerals (e.g., > 3999).
