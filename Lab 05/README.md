# Lab 05 – Software Construction & Development (Lab)

**Name:** Mahdi Ali  **Roll No.:** 16
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2026  **Instructor:** Engr. Dr. Asma Javaid

## Files

| File | Description |
|------|-------------|
| `Lab 05_Mahdi Ali_16.docx` | Main submission: explanation, screenshots, test cases and code for Q1 and Q2 |
| `code_lab5/q1_login.py` | Q1 – Login page (CNIC + Password) |
| `code_lab5/q2_form.py` | Q2 – Registration form |
| `README_Lab05.md` | This file |

## Requirements

- Python 3.8 or newer with Tkinter (included with the standard Python installer on Windows and macOS; on Ubuntu: `sudo apt install python3-tk`)
- `tkcalendar` (needed only for Q2's DatePicker): `pip install tkcalendar`

## How to run

```bash
python code_lab5/q1_login.py
python code_lab5/q2_form.py
```

## Q1 – User Login Page

- Fields: **CNIC** and **Password** (masked, with a "Show password" checkbox).
- Hard-coded credentials: CNIC `12345-6789012-3`, Password `admin123`.
- Checks: both fields filled, CNIC in the format `XXXXX-XXXXXXX-X`, then credentials match.
- Success shows an information message box; failure shows an error message box.

## Q2 – Registration Form

Controls: First Name \*, Last Name \*, Gender (radio buttons), DOB (date picker), five Hobby checkboxes, Submit button.

| Rule | Implementation |
|------|----------------|
| a. Fields with \* are mandatory | Error box if First or Last Name is empty |
| b. Male checked by default | Gender variable initialised to `Male` |
| c. DOB default = today, min 1 Oct 1950, max today | `DateEntry(mindate=1950-10-01, maxdate=today)`, default set to today |
| d. Submit click event, valid form shows info box | `on_submit()` shows an Information message box: `Welcome Firstname Lastname` |

## Notes
- Both programs were run and tested before submission (screenshots are in the Word file).
- Everything is the student's own work, as required by the lab instructions.
