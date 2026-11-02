# Lab 3: Sequence Diagrams

**University of Azad Jammu and Kashmir, Muzaffarabad**
Department of Software Engineering
Course: Software Construction & Development (Lab)
Instructor: Engr. Dr Asma Javaid
Semester: Fall 2026

## Overview

This lab models the dynamic behaviour of two systems using UML sequence diagrams.

| Question | System modelled |
|---|---|
| Q1 | Data processing when a customer withdraws cash from an ATM |
| Q2 | Online ticket reservation system |

## Contents

| File | Description |
|---|---|
| `Lab_3_Report.docx` | The full lab report (7 pages, A4) |
| `README.md` | This file |

## Report structure

1. **Objective and notation**: what a sequence diagram is and the symbols used.
2. **Q1, ATM cash withdrawal**: participants, assumptions, flow description, and Figure 1.
3. **Q2, Online ticket reservation**: participants, assumptions, flow description, and Figure 2.
4. **Conclusion**.

The two diagrams are on landscape pages so that the labels stay readable.

## Diagram summaries

### Q1: ATM cash withdrawal
- **Participants:** Customer, ATM Interface, Bank Server, Account Database, Cash Dispenser.
- **Main flow:** insert card, enter PIN, authenticate, choose amount, check balance.
- **Alt fragment:** if the balance and daily limit allow, the account is debited and cash, receipt and card are returned. Otherwise the withdrawal is declined and the card is ejected.

### Q2: Online ticket reservation
- **Participants:** Customer, Web Interface, Reservation System, Ticket Database, Payment Gateway, Notification Service.
- **Main flow:** search trips, check availability, select and lock seats, enter details, pay.
- **Alt fragment:** if payment is approved, the booking is confirmed, the ticket saved, and a confirmation sent. If declined, the locked seats are released and the customer can retry.

## Notation

- Solid arrow: request or call message.
- Dashed arrow: return message.
- Dashed vertical line: lifeline (time flows downward).
- `alt` frame: alternative flows, where only one branch runs.

## Before submitting

Fill in these fields on the cover page of the report:
- Student Name
- Roll Number
- Course Code (the lab sheet shows only "SE-")

## Notes

- The ATM diagram assumes a valid card and correct PIN. Wrong-PIN handling is outside its scope.
- The ticket diagram assumes seats are locked temporarily during payment to prevent double booking.
