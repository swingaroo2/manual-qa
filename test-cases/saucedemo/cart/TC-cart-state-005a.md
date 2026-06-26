# TC-cart-st-005a.md

**Title:** TC-cart-st-005a
**Transition under test:** S3 + Remove Item [count == 2] => S2
**Feature or component under test:** Saucedemo inventory page -- cart
**Design technique used:** state transition
**Linked charter or requirement:** n/a
**Priority:** n/a

## Preconditions

Cart must be actionable and already have two items in it. Cart badge shows quantity 2.

## Test Data

Account: standard_user / secret_sauce

State Transition table: `state-table-cart.md`

## Steps

1. Load inventory page
2. Select "Remove" on an inventory item

## Expected Result

Cart badge updates from 2 to 1

## Actual Result

Cart badge updates from 2 to 1

## Status

pass
