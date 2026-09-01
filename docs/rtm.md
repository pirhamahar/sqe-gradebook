# GradeBook — Requirements Traceability Matrix

| Requirement ID | Requirement | Linked Test Case IDs | Status |
|---|---|---|---|
| REQ-01 | The system shall allow adding a valid numeric score. | TC-01, TC-09, TC-10 | Covered |
| REQ-02 | The system shall reject negative scores. | TC-02 | Covered |
| REQ-03 | The system shall reject non-numeric scores. | TC-03 | Covered |
| REQ-04 | The system shall calculate the average of student scores correctly. | TC-04, TC-05, TC-06 | Covered |
| REQ-05 | The system shall reject duplicate roll numbers. | TC-07 | Covered |
| REQ-06 | Student name matching shall be case-insensitive. | TC-08 | Covered |
| REQ-07 | The system shall convert numeric scores into the correct grade letter. | TC-11, TC-12 | Covered |
| REQ-08 | The system shall handle minimum and maximum valid score boundaries (0 and 100). | TC-09, TC-10 | Covered |

## Traceability Gap Check

All 8 requirements have at least one linked test case. Therefore, there are **zero requirements with missing test coverage**.

The previous coverage gap for grade-letter conversion was closed by linking **TC-11** (mid-range grade conversion) and **TC-12** (boundary grade conversion) to REQ-07.
