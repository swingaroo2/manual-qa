# Test Case: TC-login-004

**Title:** P4: Empty password
**Feature or component under test:** saucedemo login page
**Design technique used:** equivalence partitioning
**Linked charter or requirement:** n/a
**Priority:** high

## Preconditions

Login screen must be loaded in fresh, with empty username and password fields. Text fields and Login button must be actionable.

## Test Data

### Partitions

1. Valid credentials
2. Invalid credentials
3. Empty username
4. Empty password
5. Locked out user

Representative pair chosen: valid username + empty password

## Steps

1. load login screen
2. enter valid username `!standard_user`
3. leave password field blank
4. click Login button

## Expected Result

User credentials are rejected. User is presented with error message _"Epic sadface: Password is required"_.

## Actual Result

User credentials are rejected. User is presented with error message _"Epic sadface: Password is required"_.

## Status

pass
