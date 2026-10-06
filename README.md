# PL/SQL GOTO Statements and Functions

**Individual Assignment III — Database Development with PL/SQL (INSY 8311)**

| | |
|---|---|
| **Student** | Kenneth |
| **Student ID** | 20252SEN344 |
| **University** | Adventist University of Central Africa (AUCA) |
| **Instructor** | Eric Maniraguha |
| **Assignment date** | Thursday, October 1, 2026 |
| **Deadline** | Thursday, October 8, 2026 at 11:59 PM |

---

## 1. Overview

This repository contains my individual practical work on:

- PL/SQL `GOTO` statements (including illegal uses and how to fix them)
- Stored functions
- Exception handling
- Using functions inside SQL queries
- Organizing and documenting work on GitHub

The work is divided into three parts: **Part A (GOTO)**, **Part B (Functions)**, and **Part C (Combined Task)**.

---

## 2. Repository Structure

```
plsql-goto-functions-20252SEN344-kenneth/
│
├── README.md
├── .gitignore
├── 00_setup/
│   └── create_tables.sql
├── 01_goto/
│   ├── A1_number_classifier.sql
│   ├── A2_salary_review.sql
│   ├── A3_illegal_goto.sql
│   └── A4_rewrite_no_goto.sql
├── 02_functions/
│   ├── B1_fn_annual_salary.sql
│   ├── B2_fn_years_of_service.sql
│   ├── B3_fn_calculate_tax.sql
│   ├── B4_fn_dept_name.sql
│   └── C1_fn_validate_payroll.sql
├── 03_tests/
│   ├── B5_functions_in_select.sql
│   ├── test_functions.sql
│   └── test_validate_payroll.sql
├── screenshots/
│   ├── A1_output.png
│   ├── A2_output.png
│   ├── A3_error_and_fix.png
│   ├── A4_output.png
│   ├── B5_select_output.png
│   └── C1_output.png
└── docs/
    └── REFLECTION.md
```

---

## 3. Task Summary

### Part A — GOTO Statements (`01_goto/`)

| Task | File | Description |
|------|------|-------------|
| A1 | `A1_number_classifier.sql` | Classifies a number using `GOTO` to jump to the matching label. |
| A2 | `A2_salary_review.sql` | Reviews a salary and uses `GOTO` to branch to the correct outcome. |
| A3 | `A3_illegal_goto.sql` | Demonstrates an illegal `GOTO` (compile error), then shows the fix. |
| A4 | `A4_rewrite_no_goto.sql` | Rewrites a GOTO-based program using structured control flow (`IF/ELSIF`, loops). |

### Part B — Functions (`02_functions/` and `03_tests/`)

| Task | File | Description |
|------|------|-------------|
| B1 | `B1_fn_annual_salary.sql` | Function that returns the annual salary of an employee. |
| B2 | `B2_fn_years_of_service.sql` | Function that returns an employee's years of service. |
| B3 | `B3_fn_calculate_tax.sql` | Function that calculates tax from a salary. |
| B4 | `B4_fn_dept_name.sql` | Function that returns a department name from its ID. |
| B5 | `B5_functions_in_select.sql` | Calls the functions above directly inside a `SELECT` statement. |

### Part C — Combined Task

| Task | File | Description |
|------|------|-------------|
| C1 | `C1_fn_validate_payroll.sql` | Payroll validator that combines functions, validation logic, and exception handling. |
| C2 | `docs/REFLECTION.md` | Written reflection on what I learned. |

---

## 4. How to Run

Run the scripts in this order:

1. **Setup:** run `00_setup/create_tables.sql` to create and populate the tables.
2. **Functions:** compile all scripts in `02_functions/`.
3. **GOTO programs:** run the programs in `01_goto/`.
4. **Tests:** run the test files in `03_tests/`.
5. **Verify:** compare the results with the screenshots in `screenshots/`.

> Tip: enable output first with `SET SERVEROUTPUT ON;` so `DBMS_OUTPUT.PUT_LINE` results are visible.

---

## 5. Screenshots

| Task | Screenshot |
|------|-----------|
| A1 | `screenshots/A1_output.png` |
| A2 | `screenshots/A2_output.png` |
| A3 (error and fix) | `screenshots/A3_error_and_fix.png` |
| A4 | `screenshots/A4_output.png` |
| B5 | `screenshots/B5_select_output.png` |
| C1 | `screenshots/C1_output.png` |

---

## 6. Notes — AI Usage Disclosure

In line with the course's academic integrity policy, I am disclosing my use of an AI assistant.

**AI used:** Claude (by Anthropic)

**How I used it:**
- To read the assignment brief and help me turn its requirements into a clear, complete README.md.
- To help me understand concepts such as `GOTO` label rules, why some jumps are illegal in PL/SQL, and how functions can be called from SQL.
- To check my understanding while preparing for the quiz.

**Why I chose Claude over other AI tools:**

1. **It works well with long, structured documents.** The assignment brief has strict rules, a required folder structure, and a checklist. Claude followed these details closely, so nothing required was missed.
2. **It explains the reasoning, not just the answer.** This assignment is followed by a quiz, so I need to understand *why* code works. Claude's step-by-step explanations helped me learn the concepts instead of just copying results.
3. **Its answers are clear and to the point.** I prefer concise, direct responses. Claude gives focused answers without unnecessary filler, which saves time when studying.
4. **It is honest about uncertainty.** When something depends on my environment (for example, my Oracle version or table design), Claude says so rather than guessing. This pushed me to test everything myself and not trust any output blindly.
5. **It supports learning, not just completing.** It handles both writing/formatting tasks (like this README) and technical explanations in one place, which kept my workflow simple.

**My responsibility:** AI was a support tool. I wrote, ran, and tested my SQL code myself, and I understand and can explain everything submitted in this repository.

---

## 7. Final Checklist

- [x] Public GitHub repository
- [x] Correct repository name (`plsql-goto-functions-20252SEN344-kenneth`)
- [x] All required SQL files completed
- [x] Functions compile successfully
- [x] Tests completed
- [x] Screenshots included
- [x] Reflection completed
- [x] README completed
- [x] At least 5 meaningful commits
- [x] GitHub link submitted through the Google Form
- [x] Prepared for next week's quiz

---

## 8. Submission

The link to this public repository is submitted through the official Google Form before **Thursday, October 8, 2026 at 11:59 PM**. No email submission was made.
