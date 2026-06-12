# Test Case: TC-login-011

**Title:** (p7/4) blocked username + invalid password
**Feature or component under test:** saucedemo login page
**Design technique used:** equivalence partitioning
**Linked charter or requirement:** n/a
**Priority:** high

## Preconditions

Login screen must be loaded in fresh, with empty username and password fields. Login button must be actionable.

## Test Data

### Partitions
1. valid username (standard_user, problem_user, performance_glitch_user, error_user, visual_user)
2. valid password (secret_sauce)
3. invalid username (invalid_user)
4. invalid password (!secret_sauce, or even attempted SQL injection)
5. empty username ("")
6. empty password ("")
7. blocked username (locked_out_user)

Thought process: see `TC-login-001`

## Steps

1. load login screen
2. enter username `locked_out_user`
3. enter password `!secret_sauce`
4. click Login button

## Expected Result

User credentials are rejected. User is presented with error message *"Epic sadface: Username and password do not match any user in this service"*.

## Actual Result
 
User credentials are rejected. User is presented with error message *"Epic sadface: Username and password do not match any user in this service"*.

## Status

pass