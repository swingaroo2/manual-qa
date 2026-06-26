# TC-cart-st-002.md

**Title:** TC-cart-st-002
**Transition under test:** S1 + Remove Item -> invalid
**Feature or component under test:** Saucedemo inventory page -- cart
**Design technique used:** state transition
**Linked charter or requirement:** n/a
**Priority:** n/a

## Preconditions

Cart must be actionable and empty

## Test Data

Account: standard_user / secret_sauce

State Transition table: `state-table-cart.md`

## Steps

1. Load inventory page
2. Select "Remove" on an inventory item

## Expected Result

No interaction with a Remove button is possible as this button is not visible/actionable. This is an invalid transition.

## Actual Result

No interaction with a Remove button is possible as this button is not visible/actionable. This is an invalid transition.

## Status

pass
