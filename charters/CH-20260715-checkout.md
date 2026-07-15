# Exploratory Charter: CH-20260715-feature

**Charter:** Checkout: Overview: Validating Total calculation

**Areas in scope:** saucedemo checkout, with multiple users

**Tester:** Me
**Date:** 2026-06-27
**Timebox:** 5-10 minutes (short session)

## Test Notes

Running notes of what you tried, observed, and questioned. Capture as you go, not after.

Assumption under test: Total calculation looks stable across users

- `standard_user`: data display correctly calculated
- `performance_glitch_user`: data display correctly calculated
- `error_user`: erroneously navigates to Checkout: Overview despite Last Name not having a value (this should be an error)
- `visual_user`: data display correctly calculated, multiple visual bugs upstream of Checkout: Overview (this charter only writes up bugs in Areas in scope)

Note: On `standard_user` and `visual_user`, multiple cart items sum to a correct Total. All users tested with one cart item, these two users also tested with multiple.

## Bugs Found

List each with its bug report ID.

## Issues and Questions

Unable to test Checkout: Overview with the following users

- `locked_out_user`: locked out of system, by design (not a bug)
- `problem_user`: text entry bug in Checkout: Your Information

`problem_user` may represent a change in behavior on saucedemo. Previous bug write-ups note Checkout: Overview was tested with this user. Need version history access or dev team contact to investigate further.

## Coverage and Data

See Test Notes for users exercised in test

## Session Debrief

Checkout: Overflow is stable with users able to access it. Errors encountered were upstream of this page. No defects to write up for this page.
