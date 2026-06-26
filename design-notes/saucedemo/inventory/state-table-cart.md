# State Transition Table for Cart Badge

| States    | Add Item | Remove Item                             |
| --------- | -------- | --------------------------------------- |
| S1: Empty | S2       |                                         |
| S2: One   | S3       | S1                                      |
| S3: Many  | S3       | [count == 2] -> S2 or [count > 2] -> S3 |

ISTQB syllabus says "[i]ts rows represent states, and its columns represent events".
