# Test Case: TC-login-003

**Title:** empty username + empty password

**Feature or component under test:** Login Page

**Design technique used:** equivalence partitioning
- black box testing technique
- splits data into partitions
- data in each partition should cause the same system behavior

**Linked charter or requirement:**

**Priority:** high
- rationale: if user can't get past login screen, they're blocked from the entire system
- if unauth'd user logs in, they can cause damage or steal data

## Preconditions
- username and password fields are enabled, visible, interactable, and empty
- login button is enabled, visible, interactable

## Test Data

### Partitions
1. valid username + valid password
2. valid username + invalid password
3. valid username + empty password
4. invalid username + valid password
5. invalid username + invalid password
6. invalid username + empty password
7. empty username + empty password

chosen partition: 7

## Steps

1. click Login button

## Expected Result

1. underlines of username/password fields turn red
2. red circles with white x appear next to username/password fields
3. error view appears with white x in top right, with message "Epic sadface: Username is required"

## Actual Result

Filled in at execution time.

## Status

not run / pass / fail / blocked
