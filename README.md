# Lecture 8 – Fixing a Buggy Python Script Using AI

## Overview
This practical demonstrates unit testing, debugging, and the RED → FIX → GREEN cycle in Python.

## Files
- `student_utils.py`: Contains functions to calculate averages, check passing marks, and assign grades.
- `test_student_utils.py`: Contains nine unit tests for the expected behaviour.
- `red_output.txt`: Records the test failures before fixing the bugs.
- `green_output.txt`: Records the successful test results after fixing the bugs.
- `bug_notes.md`: Documents the bugs, their causes, and their fixes.
- `audit.md`: Contains an AI-assisted review of the corrected solution.

## How to Run the Tests
Run the following command from the directory containing both Python files:

```bash
python test_student_utils.py
```

## Bugs Fixed
1. Average calculation: changed the denominator from `len(marks) - 1` to `len(marks)`.
2. Passing boundary: changed `>` to `>=`.
3. Grade ordering: checked the Distinction condition before First and Second.

## Testing Results
- Number of tests: 9
- Final result: All nine tests pass.

## RED → FIX → GREEN
- RED: Run the tests against the buggy implementation and capture the failures.
- FIX: Correct the implementation without changing the tests.
- GREEN: Rerun the same test suite and verify that all tests pass.
