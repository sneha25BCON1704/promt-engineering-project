# Prompt Engineering - Lecture 8: Debugging & Unit Testing

## Overview
This repository contains the debugging assignment for Lecture 8 following the **RED -> FIX -> GREEN** cycle using Google Colab and Python `unittest`.

- **Files Included:** `student_utils.py`, `test_student_utils.py`
- **Total Tests:** 9 tests
- **Final Result:** All 9 tests passing (GREEN phase)

## How to Run Tests
Run the test suite using the following command in your terminal or Colab:
```bash
python test_student_utils.py
### Step 4: Create a `bug_notes.md` File
Create a new file named `bug_notes.md` in your repository and paste this bug table (required for your submission)[cite: 6]:

```markdown
# Bug Notes & Audit Log

| Bug | Evidence / Failed Test | Cause | Fix |
| :--- | :--- | :--- | :--- |
| **Average Calculation** | 135.0 instead of 90.0; single-mark division crash | Dividing by `len(marks) - 1` | Changed denominator to `len(marks)`[cite: 6] |
| **Pass Boundary** | 40 returned `False` | Used strict greater-than (`>`) instead of greater-than-or-equal (`>=`) | Used `>= PASS_MARK`[cite: 6] |
| **Grade Ordering** | 95 returned "First" instead of "Distinction" | `>= 60` was checked before `>= 90` | Checked `>= 90` first in the conditional tree[cite: 6] |
