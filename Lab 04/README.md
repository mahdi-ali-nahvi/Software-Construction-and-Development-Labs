# Lab 04 – Software Construction & Development (Lab)

**Name:** Mahdi Ali  **Roll No.:** 16
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2026  **Instructor:** Engr. Dr Asma Javaid

## Files

| File | Description |
|------|-------------|
| `Lab 04_Mahdi Ali_16.docx` | Main submission: answers to Q1, Q2 and Q3 with UML diagrams, C++ code and output |
| `code/q2_animal.cpp` | Q2 – Animal / Cat / Dog inheritance |
| `code/q3_shape.cpp` | Q3 – Shape / Triangle / Rectangle inheritance |
| `README.md` | This file |

## Summary of tasks

### Q1 – Online Doctor Appointment Management System
Identified classes: **User** (abstract), **Patient**, **Doctor**, **Appointment**, **Schedule**, **Notification**, **Hospital**.
The Word file explains each class and gives a UML class diagram for each one, plus a combined diagram showing:
- Patient and Doctor inherit from User
- Patient 1..0..* Appointment, Doctor 1..0..* Appointment
- Doctor 1..1..* Schedule
- Appointment triggers Notification (confirmation on accept, rejection on reject)
- Appointment is held at a Hospital

### Q2 – Animal, Cat, Dog
`Animal` has `eat()` and `sleep()`. `Cat` adds `meow()`, `Dog` adds `bark()`. Both inherit publicly from `Animal`.

### Q3 – Shape, Triangle, Rectangle
`Shape` is abstract (pure virtual `input()`, `area()`, `display()`).
`Triangle` (½ × base × height) and `Rectangle` (length × width) read values from the user and print their area.

## How to compile and run

Requires a C++ compiler (g++ 11 or newer recommended, C++11 or later).

```bash
g++ -o q2 code/q2_animal.cpp && ./q2
g++ -o q3 code/q3_shape.cpp && ./q3
```

Example input for Q3: `10 5 7 4` (base, height, length, width) gives Triangle area = 25 and Rectangle area = 28.

## Notes
- Both programs were compiled and tested before submission.
- Everything is the student's own work, as required by the lab instructions.
