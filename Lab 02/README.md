# Lab 2: Activity & State Machine Diagrams

**Course:** Software Construction & Development (Lab), SE-3102
**Department:** Software Engineering, University of Azad Jammu and Kashmir, Muzaffarabad
**Semester:** Fall 2022  |  **Instructor:** Engr. Saba Naseem

## Tasks Covered

| Q | Task | Diagram type | Output |
|---|------|--------------|--------|
| 1 | foodPanda (online food order app) process using swimlanes | Activity diagram with swimlanes | `diagrams/Q1_foodpanda_activity_swimlane.png` |
| 2 | Toaster: states, activities in each state, triggered and triggerless events/actions | State diagram | `diagrams/Q2_toaster_state_diagram.png` |
| 3 | Elevator/Lift | State machine diagram | `diagrams/Q3_elevator_state_machine.png` |

## Files

```
Lab_02_Report.docx          Main deliverable: full report (Word), diagrams + explanations
README.md                   This file
diagrams/                   The three diagrams as PNG images
scripts/
  q1_activity_swimlane.py   Generates the Q1 diagram (Python + matplotlib)
  q2_q3_state_diagrams.py   Generates the Q2 and Q3 diagrams (Python + Graphviz)
  dot_sources/              Graphviz .dot sources for Q2 and Q3
  build_report.js           Builds the Word report (Node.js + docx)
```

## Report Contents

1. **Cover details and objective**: course info and a summary of tasks
2. **Q1**: swimlane table, notation used, diagram, step-by-step explanation (including the payment-failure and restaurant-rejection alternative flows)
3. **Q2**: state-diagram concepts, table of entry / do / exit activities per state, diagram, transition table classified as triggered or triggerless, explanation
4. **Q3**: assumptions, state descriptions, diagram, transition table (event / guard / action), explanation and a worked scenario
5. **Conclusion**

## Before Submitting

Fill in your **Student Name**, **Registration No.** and **Submission Date** in the table on page 1 of `Lab_02_Report.docx`.
As the lab sheet states, upload the work on **QOBE** (not by email or WhatsApp) and submit before the deadline.

## Re-generating (optional)

Requirements: Python 3 with `matplotlib`, Graphviz (`dot`), Node.js with the `docx` package.

```bash
python3 scripts/q1_activity_swimlane.py       # -> diagrams/Q1_...png
python3 scripts/q2_q3_state_diagrams.py       # -> diagrams/Q2_...png, Q3_...png
node scripts/build_report.js                  # -> Lab_02_Report.docx
```

(`build_report.js` reads image paths and sizes from `/home/claude/img.json`; adjust the paths at the top of the script if running elsewhere.)

## Diagram Legend

- **Q1:** filled circle = start, circle with dot = end, rounded box = action, diamond = decision, coloured bands = swimlanes.
- **Q2:** solid black arrow = *triggered* transition (`event [guard] / action`); dashed red arrow = *triggerless* (completion) transition.
- **Q3:** `event [guard] / action` labels on every arrow; self-loops show events that do not change the state.
