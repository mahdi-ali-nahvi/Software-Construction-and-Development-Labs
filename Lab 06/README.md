# Lab 06 – Software Construction & Development (Lab) – SE-3102

**Name:** Mahdi Ali  **Roll No.:** 16
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2026  **Instructor:** Engr. Dr. Asma Javaid

## Files

| File | Description |
|------|-------------|
| `Lab 06_Mahdi Ali_16.docx` | Main submission: design, screenshots, test cases and code |
| `code_lab6/calculator.py` | Q1 – Simple Calculator (GUI) |
| `README_Lab06.md` | This file |

## Requirements

- Python 3.8 or newer with Tkinter (included with the standard Python installer on Windows and macOS; on Ubuntu: `sudo apt install python3-tk`)
- No extra packages needed

## How to run

```bash
python code_lab6/calculator.py
```

## Q1 – Simple Calculator

Layout follows the sample in the lab task:

```
[ 0                       ]
 7   8   9   /   CE
 4   5   6   *   C
 1   2   3   -   =
   0     .   +   =
```

- **Operations:** `+  -  *  /` on integers and decimals; chained calculations (e.g. `2 + 3 + 4 =` gives `9`).
- **CE** clears the current entry; **C** clears everything.
- **Division by zero** shows "Cannot divide by zero" (no crash).
- **Keyboard:** digits, `+ - * / .`, Enter or `=` for equals, Backspace = CE, Esc = C.
- **Structure:** `CalculatorLogic` (calculation rules, no GUI) and `CalculatorApp` (window and buttons).

## Notes
- The program was run and tested before submission (screenshots and test cases are in the Word file).
- Everything is the student's own work, as required by the lab instructions.
