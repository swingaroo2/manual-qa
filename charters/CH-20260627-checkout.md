# Exploratory Charter: CH-20260627-checkout

**Charter:** Explore the Saucedemo checkout flow to check for input validation and data handling defects, using Constraint and Input Method heuristics

**Areas in scope:** saucedemo checkout

**Tester:** Me
**Date:** 2026-06-27
**Timebox:** 30 minutes

## Test Notes

Running notes of what you tried, observed, and questioned. Capture as you go, not after.

**Login: Problem User**

Logged out after a few minutes of inactivity, probably normal?

- unable to enter text into last name field by any previously successful means (drag drop, copy paste)
  - can consistently reproduce this scenario, I was likely logged in as the standard user

Your Cart - can we enter checkout in a bad state? - products in cart link to the wrong item - QTY header looks misaligned, need to compare against `standard_user`

Checkout: Your Information

- Tab from first name > last name + text entry overwrites first name with a single character at a time
- Any typed-out text entry in last name overwrites first name
  - did not observe similar behavior in any other text field
  - copy-paste, drag-drop into last name field correctly allows text entry

## Bugs Found

BUG-0001: products in cart link to the wrong detail page item

BUG-0002: any text entry in last name field overwrites first name field with a single character at a time

## Issues and Questions

By all appearances I was able to initially enter text into the Last Name field on Your Information with `problem_user`. However, after being automatically logged out and logging back in, any attempts at entering text into the Last Name field followed the same error path as manual text entry. It's possible I was unknowingly logged in as `standard_user`. Further retesting of the text entry scenario consistently reproduced the defect, reinforcing my suspicion.

Was unable to test the rest of the checkout flow with `problem_user` as the last name field could never be filled.

## Coverage and Data

### Test Data

login: `problem_user` / `secret_sauce`

What you actually exercised, and any test data you used or need next time.

## Session Debrief

When encountering text entry defects, try multiple forms of text entry to determine if the failure path is universal to all text entry methods, or just specific ones.
