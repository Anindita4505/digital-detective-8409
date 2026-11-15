# Mission 5 — Numbers and Data

## 1. Mission Title

Numbers and Data

## 2. Task / Objective

The objective was to understand number systems, convert decimal, binary and hexadecimal values, verify conversions using Python, build a number converter program and learn how computers store text.

## 3. Work Completed

### Task 5.1 — Convert Numbers by Hand

**1. Decimal 13 to Binary**

Repeated division by 2:

| Division | Quotient | Remainder |
| -------- | -------: | --------: |
| 13 ÷ 2   |        6 |         1 |
| 6 ÷ 2    |        3 |         0 |
| 3 ÷ 2    |        1 |         1 |
| 1 ÷ 2    |        0 |         1 |

Reading the remainders from bottom to top:

**Answer: 1101₂**

**2. Decimal 25 to Binary**

| Division | Quotient | Remainder |
| -------- | -------: | --------: |
| 25 ÷ 2   |       12 |         1 |
| 12 ÷ 2   |        6 |         0 |
| 6 ÷ 2    |        3 |         0 |
| 3 ÷ 2    |        1 |         1 |
| 1 ÷ 2    |        0 |         1 |

Reading the remainders from bottom to top:

**Answer: 11001₂**

**3. Binary 1010 to Decimal**

(1 × 2³) + (0 × 2²) + (1 × 2¹) + (0 × 2⁰)

= 8 + 0 + 2 + 0

**Answer: 10₁₀**

**4. Binary 1101 to Decimal**

(1 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰)

= 8 + 4 + 0 + 1

**Answer: 13₁₀**

**5. Hexadecimal A to Decimal**

A represents 10 in hexadecimal.

**Answer: 10₁₀**

**6. Hexadecimal 1F to Decimal**

F represents 15.

(1 × 16¹) + (15 × 16⁰)

= 16 + 15

**Answer: 31₁₀**

**7. Binary 1111 to Hexadecimal**

1111₂ = 15₁₀ = F₁₆

**Answer: F₁₆**

### Task 5.2 — Verify Using Python

Used Python's built-in conversion functions to verify the manual calculations.

| Python expression | Result    | Matches manual answer? |
| ----------------- | --------- | ---------------------- |
| `bin(13)`         | `0b1101`  | Yes                    |
| `bin(25)`         | `0b11001` | Yes                    |
| `int('1010', 2)`  | `10`      | Yes                    |
| `int('1101', 2)`  | `13`      | Yes                    |
| `hex(13)`         | `0xd`     | Yes                    |
| `hex(31)`         | `0x1f`    | Yes                    |
| `int('A', 16)`    | `10`      | Yes                    |
| `int('1F', 16)`   | `31`      | Yes                    |

All Python results matched the manual calculations.

### Task 5.3 — Build a Small Number Converter

Created a Python program named `number_converter.py`.

**Program:**

```python
number = int(input("Enter a decimal number: "))

binary = bin(number)
hexadecimal = hex(number)

print("Binary:", binary)
print("Hexadecimal:", hexadecimal)
```

**Test results:**

| Input number | Binary output | Hexadecimal output |
| -----------: | ------------- | ------------------ |
|           13 | `0b1101`      | `0xd`              |
|           25 | `0b11001`     | `0x19`             |
|           42 | `0b101010`    | `0x2a`             |

All three tests were successful.

**Functions used:**

- `input()` — Accepts input from the user.
- `int()` — Converts the input string into an integer.
- `bin()` — Converts an integer into binary.
- `hex()` — Converts an integer into hexadecimal.
- `print()` — Displays the results.

### Task 5.4 — How Is Text Stored?

**1. ASCII decimal codes**

| Character   | ASCII decimal code |
| ----------- | -----------------: |
| Uppercase A |                 65 |
| Lowercase a |                 97 |

**2. Why does a computer need an encoding standard?**

A computer stores information as binary data. An encoding standard assigns numerical values to characters so computers can store, process and display text consistently.

**3. Example of a character outside basic ASCII**

The Indian Rupee symbol (₹) is not part of basic ASCII. UTF-8 can represent this character.

## 4. Commands / Tools Used

- `cd mission-05-numbers-data` — Entered the Mission 5 directory.
- `ls` — Listed the files in the directory.
- `python3` — Opened the Python interactive environment.
- `bin()` — Converted decimal integers into binary.
- `hex()` — Converted decimal integers into hexadecimal.
- `int()` — Converted binary and hexadecimal strings into decimal.
- `python3 number_converter.py` — Executed the number converter.
- Visual Studio Code — Created and edited the Python program and README.

## 5. My Understanding

I learned how decimal, binary and hexadecimal number systems work and how to convert values between them. I understood how Python's built-in functions make number conversion easier. I also learned that computers use character-encoding standards such as ASCII and UTF-8 to represent text.

## 6. Difficulties Faced

Initially, I needed to understand how to convert numbers between different number systems and how to use Python's conversion functions.

## 7. How I Resolved Them

I practised manual conversions using division and positional values, then verified my answers using Python. I also created and tested a Python program with three different positive numbers.

## 8. Evidence / Files

- `number_converter.py` — Working decimal-to-binary and decimal-to-hexadecimal converter.
- `README.md` — Manual conversions, Python verification, test results and text-encoding notes.

## 9. Commit Details

**Planned commit message:** `Build number converter and practise data representation`
