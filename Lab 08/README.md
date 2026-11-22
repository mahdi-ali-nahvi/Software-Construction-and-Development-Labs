# Lab 08 – Software Construction & Development (Lab) – SE-3102

**Name:** Mahdi Ali  **Roll No.:** 16
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2026  **Instructor:** Engr. Dr. Asma Javaid
**Topic:** Exception handling with custom exceptions

## Files

| File | Description |
|------|-------------|
| `Lab 08_Mahdi Ali_16.docx` | Main submission: explanation, code, output, screenshots and test cases |
| `code_lab8/q1_coffee.py` | Q1 – Coffee temperature check (console) |
| `code_lab8/q2_hemoglobin.py` | Q2 – Hemoglobin level checker (GUI form) |
| `README_Lab08.md` | This file |

## Requirements

- Python 3.8 or newer. Q2 needs Tkinter (included with the standard Python installer on Windows and macOS; on Ubuntu: `sudo apt install python3-tk`). No extra packages.

## How to run

```bash
python code_lab8/q1_coffee.py
python code_lab8/q2_hemoglobin.py
```

## Q1 – Coffee Shop

Enter a temperature (type `q` to quit).

| Temperature | Result |
|-------------|--------|
| 85 or more | `TooHotCoffeeCupException` – prints "Too Hot Coffee Cup" |
| 66 to 84 | Standard – coffee is served |
| 65 or less | `TooColdCoffeeCupException` – prints "Too Cold Coffee Cup" |

Decimals such as 84.5 fall between the limits and are treated as standard. Non-numeric input is rejected.

## Q2 – Hemoglobin Level Checker

Choose Man / Woman / Child, enter the Hb level in g/dL and click **Check Hb Level**.

| Patient | Normal range (g/dL) |
|---------|--------------------|
| Man | 13.5 – 17.5 |
| Woman | 12.0 – 15.5 |
| Child | 11.5 – 15.5 (general range) |

- Below the range → `LowHemoglobinException` (possible anemia)
- Above the range → `HighHemoglobinException`
- Both extend a base `HemoglobinException`; invalid input (not a number, 0, negative, over 30) shows an error message.

The ranges are common general reference values; exact limits vary slightly between laboratories and with a child's age. They can be changed in the `NORMAL_RANGES` dictionary.

## Notes
- Both programs were run and tested before submission (output, screenshots and test cases are in the Word file).
- Everything is the student's own work, as required by the lab instructions.
