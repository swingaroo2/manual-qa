# TC-cart-st-004.md

**Title:** TC-cart-st-004
**Transition under test:** S2 + Remove Item => S1
**Feature or component under test:** Saucedemo inventory page -- cart
**Design technique used:** state transition
**Linked charter or requirement:** n/a
**Priority:** n/a

## Preconditions

Cart must be actionable and already have one item in it. Cart badge shows quantity 1.

## Test Data

Account: standard_user / secret_sauce

State Transition table: `state-table-cart.md`

## Steps

1. Load inventory page
2. Select "Remove" on an inventory item

## Expected Result

Cart badge disappears

## Actual Result

Cart badge disappears

## Status

pass
