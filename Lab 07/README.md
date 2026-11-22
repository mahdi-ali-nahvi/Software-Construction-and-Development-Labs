# Lab 07 – Software Construction & Development (Lab) – SE-3102

**Name:** Mahdi Ali  **Roll No.:** 16
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2026  **Instructor:** Engr. Dr. Asma Javaid

## Files

| File | Description |
|------|-------------|
| `Lab 07_Mahdi Ali_16.docx` | Main submission: explanation, screenshots, test cases, sample invoice and code |
| `code_lab7/carpet_estimator.py` | Q1 – Carpet cost estimator and invoice generator |
| `README_Lab07.md` | This file |

## Requirements

- Python 3.8 or newer with Tkinter (included with the standard Python installer on Windows and macOS; on Ubuntu: `sudo apt install python3-tk`)
- No extra packages needed

## How to run

```bash
python code_lab7/carpet_estimator.py
```

## Q1 – Carpet Cost Estimator

1. Enter the customer name (optional), room length and width in feet, and choose a carpet type.
2. Click **Calculate** to see area, subtotal, tax and final cost.
3. Click **Generate Invoice** to open the invoice window; use **Save Invoice (.txt)** to keep a copy.

### Predetermined prices (Rs. per sq ft)

| Carpet type | Price |
|-------------|-------|
| Nylon Standard | 150 |
| Polyester | 200 |
| Shaggy | 260 |
| Pure Wool | 350 |
| Persian Silk | 600 |

### Rules

- Area = length × width; Subtotal = area × price
- Subtotal **below Rs. 30000** → **10%** tax; otherwise (30000 or more) → **15%** tax
- Final cost = subtotal + tax
- Input must be a positive number (max 1000 ft) and a carpet type must be selected

Example: 12 ft × 10 ft Pure Wool → 120 sq ft × 350 = Rs. 42,000 + 15% tax (Rs. 6,300) = **Rs. 48,300**.

## Notes
- The shop name, address and prices are sample values and can be changed at the top of `carpet_estimator.py`.
- The program was run and tested before submission (screenshots and test cases are in the Word file).
- Everything is the student's own work, as required by the lab instructions.
