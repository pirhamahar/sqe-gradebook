| ID | Title | Requirement | Preconditions | Steps | Expected | Priority | Type |
|---|---|---|---|---|---|---|---|
| TC-01 | Add valid score | add_score accepts valid numeric scores | Student exists | 1. Create student. 2. Call add_score(85). | Score 85 is added successfully. | High | Positive |
| TC-02 | Reject negative score | add_score rejects negative input | Student exists | 1. Create student. 2. Call add_score(-10). | Negative score is rejected with an appropriate error. | High | Negative |
| TC-03 | Reject non-numeric score | add_score rejects non-numeric input | Student exists | 1. Create student. 2. Call add_score("abc"). | Non-numeric score is rejected with an appropriate error. | High | Negative |
| TC-04 | Calculate average with scores | average() returns the average of existing scores | Student has scores 70, 80, 90 | 1. Add scores 70, 80, and 90. 2. Call average(). | Average returned is 80. | High | Positive |
| TC-05 | Average with empty list | average() handles no scores | Student has no scores | 1. Create student without scores. 2. Call average(). | Empty-score condition is handled without an incorrect average result. | High | Negative |
| TC-06 | Average with single score | average() works with one score | Student exists | 1. Add score 75. 2. Call average(). | Average returned is 75. | Medium | Positive |
| TC-07 | Reject duplicate roll number | Roll numbers must be unique | A student with roll number 101 exists | 1. Create first student with roll number 101. 2. Create another student with roll number 101. | Duplicate roll number is rejected. | High | Negative |
| TC-08 | Name case-insensitivity | Student name matching is case-insensitive | Student named Ali exists | 1. Store/search for student as "Ali". 2. Repeat using "ali" and "ALI". | All case variations identify the same student. | Medium | Positive |
| TC-09 | Accept maximum score 100 | add_score accepts maximum valid score | Student exists | 1. Call add_score(100). | Score 100 is accepted and stored. | High | Boundary |
| TC-10 | Accept minimum score 0 | add_score accepts minimum valid score | Student exists | 1. Call add_score(0). | Score 0 is accepted and stored. | High | Boundary |
| TC-11 | Convert mid-range score to grade letter | Grade conversion returns correct letter for mid-range score | Student has a mid-range score of 75 | 1. Add score 75. 2. Convert the score to a grade letter. | The correct grade letter for 75 is returned. | Medium | Positive |
| TC-12 | Convert boundary score to grade letter | Grade conversion handles a grade boundary correctly | Student has a score at a defined grade boundary | 1. Add a score at the grade boundary, such as 80. 2. Convert the score to a grade letter. | The grade letter matches the defined boundary rule. | High | Boundary |
