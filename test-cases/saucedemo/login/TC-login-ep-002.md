# Test Case: TC-login-002

**Title:** P2: Invalid credentials
**Feature or component under test:** saucedemo login page
**Design technique used:** equivalence partitioning
**Linked charter or requirement:** n/a
**Priority:** high

## Preconditions

Login screen must be loaded in fresh, with empty username and password fields. Text fields and Login button must be actionable.

## Test Data

### Partitions (outcome based)

1. Valid credentials
2. Invalid credentials
3. Empty username
4. Empty password
5. Locked out user

Representative pair chosen: valid username + invalid password

## Steps

1. load login screen
2. enter valid username `standard_user`
3. enter invalid password `!secret_sauce`
4. click Login button

## Expected Result

User credentials are rejected. User is presented with error message _"Epic sadface: Username and password do not match any user in this service"_.

## Actual Result

User credentials are rejected. User is presented with error message _"Epic sadface: Username and password do not match any user in this service"_.

## Status

pass
