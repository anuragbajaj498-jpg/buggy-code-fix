# Bug Notes – Lecture 8

| Bug | Evidence / Failed Test | Cause | Fix |
|---|---|---|---|
| Average calculation | 135.0 instead of 90.0; single-mark crash | Dividing by `len(marks) - 1` | Divide by `len(marks)` |
| Pass boundary | 40 returned False | Used `>` instead of `>=` | Use `>= PASS_MARK` |
| Distinction | 95 returned First | `>= 60` was checked before `>= 90` | Check `>= 90` first |

## Summary
Three logical bugs were identified using unit tests. The implementation was corrected without weakening or changing the tests. The same nine tests were then rerun to verify the fixes.
