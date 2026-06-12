# Test Case: TC-login-001

**Title:** (p1/2) valid username + valid password
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

Thought process: my differentiator here is whether each partition allows login -- or if not, the nature of the failure. There are multiple failure modes that present different error messages, and I created separate partitions for each one.

I am knowingly breaking the 'non-overlapping' partitions rule here since partitions 5 and 6 result in different error messages. I'm priorizing coverage over theory, given the contradiction between non-overlapping partitions, and the equivalence aspect of equivalence partitioning.

I have a feeling I did my partitions wrong. I wasn't sure how partitioning works in this scenario. Specifically breaking username and password into separate partitions vs partitioning based on username/password combos.

## Steps

1. load login screen
2. enter username `standard_user`
3. enter password `secret_sauce`
4. click Login button

## Expected Result

User credentials are accepted and user is taken to Products page.

## Actual Result

User credentials are accepted and user is taken to Products page.

## Status

pass
