# Mission 5 — Numbers and Data

## 1. Task / Objective

The objective of this mission was to understand number systems, practise converting numbers between decimal, binary and hexadecimal, use Python's built-in conversion functions, build a number converter program, and learn how computers represent text using character encoding.

## 2. Work Completed

### Task 5.1 — Convert Numbers Manually

**1. Decimal 13 to Binary**

Repeated division by 2:

- 13 ÷ 2 = 6, remainder 1
- 6 ÷ 2 = 3, remainder 0
- 3 ÷ 2 = 1, remainder 1
- 1 ÷ 2 = 0, remainder 1

Reading the remainders from bottom to top:

**(13)₁₀ = (1101)₂**

**2. Decimal 25 to Binary**

- 25 = 16 + 8 + 1
- 25 = 1(16) + 1(8) + 0(4) + 0(2) + 1(1)

**(25)₁₀ = (11001)₂**

**3. Binary 1010 to Decimal**

- 1010₂ = 1(2³) + 0(2²) + 1(2¹) + 0(2⁰)
- = 8 + 0 + 2 + 0
- = 10

**(1010)₂ = (10)₁₀**

**4. Binary 1101 to Decimal**

- 1101₂ = 1(2³) + 1(2²) + 0(2¹) + 1(2⁰)
- = 8 + 4 + 0 + 1
- = 13

**(1101)₂ = (13)₁₀**

**5. Hexadecimal A to Decimal**

- A = 10
- A × 16⁰ = 10 × 1 = 10

**(A)₁₆ = (10)₁₀**

**6. Hexadecimal 1F to Decimal**

- 1F₁₆ = 1(16¹) + 15(16⁰)
- = 16 + 15
- = 31

**(1F)₁₆ = (31)₁₀**

**7. Binary 1111 to Hexadecimal**

- 1111₂ = 8 + 4 + 2 + 1 = 15
- The hexadecimal digit representing 15 is F.

**(1111)₂ = (F)₁₆**

### Task 5.2 — Verify Using Python

The manual calculations were checked using Python's built-in conversion functions.

| Python expression | Result      | Matches manual calculation? |
| ----------------- | ----------- | --------------------------- |
| `bin(13)`         | `'0b1101'`  | Yes                         |
| `bin(25)`         | `'0b11001'` | Yes                         |
| `int("1010", 2)`  | `10`        | Yes                         |
| `int("1101", 2)`  | `13`        | Yes                         |
| `hex(10)`         | `'0xa'`     | Yes                         |
| `hex(31)`         | `'0x1f'`    | Yes                         |
| `int("A", 16)`    | `10`        | Yes                         |
| `int("1F", 16)`   | `31`        | Yes                         |

Python uses `0b` as a binary prefix and `0x` as a hexadecimal prefix.

### Task 5.3 — Build a Small Number Converter

Created the Python program `number_converter.py`.

The program asks the user to enter a positive decimal number, converts it into binary and hexadecimal, and displays both results.

**Test results:**

| Decimal input | Binary output | Hexadecimal output |
| ------------- | ------------- | ------------------ |
| 10            | 1010          | A                  |
| 25            | 11001         | 19                 |
| 31            | 11111         | 1F                 |

All three test cases produced the expected results.

### Task 5.4 — How Is Text Stored?

1. ASCII decimal code for uppercase `A`: **65**
2. ASCII decimal code for lowercase `a`: **97**

**Why do computers need a character encoding standard?**

Computers store information as binary numbers (0s and 1s). A character encoding standard assigns a numerical value to each character so computers can store, process and display text consistently.

**Example of a character not included in basic ASCII:** ₹ (Indian Rupee symbol).

Unicode supports characters from many languages and symbol systems, including characters that are not part of basic ASCII.

## 3. Commands / Tools Used

- `python3` — opened the Python interpreter and executed the converter program.
- `bin()` — converted decimal integers into binary representation.
- `int(value, 2)` — converted binary strings into decimal integers.
- `hex()` — converted decimal integers into hexadecimal representation.
- `int(value, 16)` — converted hexadecimal strings into decimal integers.
- `input()` — accepted user input.
- `print()` — displayed the converted values.
- `ls` — checked files and directories in the terminal.

## 4. My Understanding

I learned how decimal, binary and hexadecimal number systems work and how to convert numbers between them manually. I also learned how Python's built-in functions can perform these conversions.

I understood that computers represent text using character encoding standards, which map characters to numerical values.

## 5. Difficulties Faced

No major difficulties were recorded during the practical work.

## 6. How I Resolved Them

I checked the manual conversion results using Python's built-in functions and tested the number converter with three different decimal inputs to verify its output.

## 7. Evidence / Files

**Program file:**

- `mission-05-numbers-data/number_converter.py`

**Documentation:**

- `mission-05-numbers-data/README.md`

**Evidence screenshot:**

- `evidence/mission-05-number-converter.png`

## 8. Commit Details

**Commit message:** `Build number converter and practise data representation`
**Branch:** `main`
**Status:** 'Successfully committed and pushed to GitHub.'
