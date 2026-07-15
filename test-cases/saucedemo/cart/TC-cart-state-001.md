# TC-cart-st-001.md

**Title:** TC-cart-st-001
**Transition under test:** S1 (empty) + Add Item => S2 (one)
**Feature or component under test:** Saucedemo inventory page -- cart
**Design technique used:** state transition
**Linked charter or requirement:** n/a
**Priority:** n/a

## Preconditions

Cart must be actionable and empty

## Test Technique-Specific Artifacts

State Transition table: `state-table-cart.md`

## Test Data

Account: standard_user / secret_sauce

## Steps

1. Load inventory page
2. Select "Add to cart" on an inventory item

## Expected Result

Cart badge appears with quantity 1

## Actual Result

Cart badge appears with quantity 1

## Status

pass
