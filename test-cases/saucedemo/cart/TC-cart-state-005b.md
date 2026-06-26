# TC-cart-state-005b.md

**Title:** TC-cart-state-005b
**Transition under test:** S3 + Remove Item [count > 2] => S3
**Feature or component under test:** Saucedemo inventory page -- cart
**Design technique used:** state transition
**Linked charter or requirement:** n/a
**Priority:** n/a

## Preconditions

Cart must be actionable and already have three items in it. Cart badge shows quantity 3.

## Test Data

Account: standard_user / secret_sauce

State Transition table: `state-table-cart.md`

## Steps

1. Load inventory page
2. Select "Remove" on an inventory item

## Expected Result

Cart badge updates from 3 to 2

## Actual Result

Cart badge updates from 3 to 2

## Status

pass
