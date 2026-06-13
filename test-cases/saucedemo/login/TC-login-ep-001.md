# Test Case: TC-login-001

**Title:** P1: Valid Credentials
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

## Steps

1. load login screen
2. enter valid username `standard_user`
3. enter valid password `secret_sauce`
4. click Login button

## Expected Result

User credentials are accepted and user is taken to Products page.

## Actual Result

User credentials are accepted and user is taken to Products page.

## Status

pass
