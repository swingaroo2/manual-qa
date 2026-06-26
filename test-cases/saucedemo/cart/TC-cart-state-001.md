# TC-cart-st-001.md

**Title:** TC-cart-st-001
**Transition under test:** S1 + Add Item => S2
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
2. Select "Add to cart" on an inventory item

## Expected Result

Cart badge appears with quantity 1

## Actual Result

Cart badge appears with quantity 1

## Status

pass
