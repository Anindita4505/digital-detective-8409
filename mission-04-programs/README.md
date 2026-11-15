# Mission 4 — How Programs Run

## 1. Mission Title

How Programs Run

## 2. Task / Objective

The objective was to create and run a simple Python program and understand the difference between compilers and interpreters.

## 3. Work Completed

### Task 4.1 — Create and Run a Python Program

Created a Python file named `hello.py` containing:

```python
print("Hello from Python")
```

Ran the program using Python 3.

**Output:**

```text
Hello from Python
```

### Task 4.2 — Compiler vs Interpreter

| Point                              | Compiler                                     | Interpreter                                                |
| ---------------------------------- | -------------------------------------------- | ---------------------------------------------------------- |
| When translation/execution happens | Translates source code before execution.     | Translates and executes instructions during runtime.       |
| Typical output                     | Often produces an executable or object code. | Usually executes without creating a standalone executable. |
| One example                        | C compiler (GCC)                             | Python interpreter (CPython)                               |
| One advantage                      | Compiled programs can execute faster.        | Convenient for testing and debugging.                      |

**My explanation:**

A compiler translates source code into another form before the program runs. An interpreter reads and executes instructions during runtime. Compiled programs can run faster, while interpreted execution can make testing easier. Python commonly uses an interpreter, although CPython also compiles source code into bytecode before executing it.

## 4. Commands / Tools Used

- `cd mission-04-programs` — Entered the Mission 4 directory.
- `python3 hello.py` — Executed the Python program.
- Visual Studio Code — Created and edited the Python file and README.

## 5. My Understanding

I learned how to create and execute a Python program from the Terminal. I also understood that compilers translate code before execution, whereas interpreters execute instructions during runtime.

## 6. Difficulties Faced

Initially, I tried running `hello.py` from the repository's root directory, so Python could not find the file.

## 7. How I Resolved Them

I moved into the `mission-04-programs` directory and ran the command again. The program executed successfully and displayed the expected output.

## 8. Evidence / Files

- `hello.py` — Python program displaying the message.
- `README.md` — Task details and compiler/interpreter comparison.

## 9. Commit Details

**Planned commit message:** `Complete programs and compiler-interpreter mission`
