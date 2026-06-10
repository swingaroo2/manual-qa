# Test Case: TC-login-001

**Title:** valid username + valid password

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

chosen partition: 1

note: i simplified the scope of 'invalid' input for this exercise. production test cases would include partitions on malicious inputs that need to be sanitized before hitting the database

### Input Data
valid username: standard_user
valid password: secret_sauce

## Steps

1. select username field
2. enter valid username `standard_user`
3. select password field
4. enter valid password `secret_sauce`
5. click Login button

## Expected Result

Application logs in and shows Swag Labs Products page

## Actual Result

Application logs in and shows Swag Labs Products page

## Status

pass
