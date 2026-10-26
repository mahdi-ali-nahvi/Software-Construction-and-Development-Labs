# Lab 1 – Use Case Diagrams

**University of Azad Jammu and Kashmir, Muzaffarabad – Department of Software Engineering**
**Course:** Software Construction & Development (Lab) | **Semester:** Fall 2026 | **Instructor:** Engr. Dr Asma Javaid

## Overview
This lab models requirements with UML use case diagrams.

| Question | System | Actors | Use cases |
|---|---|---|---|
| Q1 | Online Ticket Reservation System | Customer, Administrator, Payment Gateway | 15 |
| Q2 | Credit Card Processing System | Customer, Vendor, Credit Card Machine | 12 |

## Files
| File | Description |
|---|---|
| `Lab_01_Report.docx` | Full lab report (actors, use cases, relationships, diagrams, explanations, conclusion) |
| `usecase_q1.png` | Use case diagram for Q1 |
| `usecase_q2.png` | Use case diagram for Q2 |
| `make_diagrams.py` | Python script that generates both diagrams |
| `README.md` | This file |

## Relationships used
**Q1**
- Book / Reserve Ticket `<<include>>` Select Seat, Make Payment, Send Confirmation
- Process Refund `<<extend>>` Cancel Reservation

**Q2**
- Swipe Card `<<include>>` Process Transaction
- Process Transaction `<<include>>` Verify Credit Limit, Update Card Balance
- Issue Balance Statement `<<include>>` Print Balance Statement / Receipt

## Regenerating the diagrams
Requires Python 3 and matplotlib.

```bash
pip install matplotlib
python make_diagrams.py
```

This writes `usecase_q1.png` and `usecase_q2.png` in the same folder.

## Drawing the diagrams yourself (for screenshots)
1. Open <https://app.diagrams.net> (draw.io) and create a blank diagram.
2. Enable **More Shapes > UML**.
3. Draw a large rectangle as the system boundary and write the system name on top.
4. Place **Actor** shapes outside the rectangle and **Ellipse** shapes (use cases) inside.
5. Join actors to use cases with solid lines (association).
6. Use dashed arrows with an open arrowhead for `<<include>>` / `<<extend>>` and label them.
   - include: arrow points from the base use case to the included one
   - extend: arrow points from the extending use case to the base one
7. Take a screenshot and paste it into the "Paste your screenshot here" boxes at the end of the report.

## Before submitting
- [ ] Fill in your name, roll number, section and course code on the cover page of the report.
- [ ] Paste your screenshots in Section 5 of the report.
- [ ] Upload on **QOBE** only (email/WhatsApp submissions are not accepted).
- [ ] Submit before the deadline; late work is not accepted.
