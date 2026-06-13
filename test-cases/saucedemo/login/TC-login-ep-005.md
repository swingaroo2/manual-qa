# Test Case: TC-login-005

**Title:** P5: Locked out user
**Feature or component under test:** saucedemo login page
**Design technique used:** equivalence partitioning
**Linked charter or requirement:** n/a
**Priority:** high

## Preconditions

Login screen must be loaded in fresh, with empty username and password fields. Login button must be actionable.

## Test Data

### Partitions

1. Valid credentials
2. Invalid credentials
3. Empty username
4. Empty password
5. Locked out user

Representative pair chosen: locked out username + valid password

## Steps

1. load login screen
2. enter locked out username `locked_out_user`
3. enter valid password `secret_sauce`
4. click Login button

## Expected Result

User credentials are rejected. User is presented with error message _"Epic sadface: Sorry, this user has been locked out."_.

## Actual Result

User credentials are rejected. User is presented with error message _"Epic sadface: Sorry, this user has been locked out."_.

## Status

pass
