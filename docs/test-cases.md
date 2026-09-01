# GradeBook — Test Cases

| ID | Title | Requirement | Preconditions | Steps | Expected | Priority | Type | Result / Note |
|---|---|---|---|---|---|---|---|---|
| TC-01 | Add valid score | add_score accepts valid numeric scores | Student exists | Create student and call add_score(85). | Score 85 is added successfully. | High | Positive |FAIL — add_score() is not implemented in the current code. GitHub Issue #1.|
| TC-02 | Reject negative score | add_score rejects negative input | Student exists | Create student and call add_score(-10). | Negative score is rejected. | High | Negative | BLOCKED — add_score() is not implemented, so rejection cannot be verified. |
| TC-03 | Reject non-numeric score | add_score rejects non-numeric input | Student exists | Create student and call add_score("abc"). | Non-numeric score is rejected. | High | Negative | BLOCKED — add_score() is not implemented, so rejection cannot be verified. |
| TC-04 | Calculate average with scores | average() returns average of existing scores | Student has scores 70, 80, 90 | Add scores and call average(). | Average returned is 80. | High | Positive | BLOCKED — average() is not implemented. |
| TC-05 | Average with empty list | average() handles no scores | Student has no scores | Create student and call average(). | Empty-score condition is handled correctly. | High | Negative | BLOCKED — average() is not implemented. |
| TC-06 | Average with single score | average() works with one score | Student exists | Add score 75 and call average(). | Average returned is 75. | Medium | Positive | BLOCKED — average() is not implemented. |
| TC-07 | Reject duplicate roll number | Roll numbers must be unique | A student with roll number 107 exists | Create two students with roll number 107. | Duplicate roll number is rejected. | High | Negative | FAIL — duplicate roll numbers are accepted by the current code. |
| TC-08 | Name case-insensitivity | Student name matching is case-insensitive | Student named Ali exists | Use Ali, ali and ALI for matching. | All case variations identify the same student. | Medium | Positive | BLOCKED — no name matching/search functionality is implemented. |
| TC-09 | Accept maximum score 100 | add_score accepts maximum valid score | Student exists | Store score 100. | Score 100 is accepted and stored. | High | Boundary | PASS — score 100 was stored successfully in the scores list. |
| TC-10 | Accept minimum score 0 | add_score accepts minimum valid score | Student exists | Store score 0. | Score 0 is accepted and stored. | High | Boundary | PASS — score 0 was stored successfully in the scores list. |
| TC-11 | Mid-range grade-letter conversion | Grade conversion returns correct letter | Student has score 75 | Convert score 75 to a grade letter. | Correct grade letter is returned. | Medium | Positive | BLOCKED — grade_letter() is not implemented. |
| TC-12 | Boundary grade-letter conversion | Grade conversion handles boundary | Student has score 80 | Convert score 80 to a grade letter. | Correct boundary grade letter is returned. | High | Boundary | BLOCKED — grade_letter() is not implemented. |
