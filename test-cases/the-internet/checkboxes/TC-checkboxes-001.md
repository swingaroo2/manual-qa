# Test Case: TC-checkboxes-001

**Title:** Ignore box 1 + Select box 2

**Feature or component under test:** Checkboxes page

**Design technique used:** equivalence partitioning

**Linked charter or requirement:** ???

**Priority:** low

## Preconditions

Page loads by default with box 1 unchecked and box 2 checked

## Test Data

### Partitions
1. select box 1 + select box 2
2. select box 1 + ignore box 2
3. ignore box 1 + select box 2
4. ignore box 1 + ignore box 2

chosen partition: 3

## Steps

1. load checkboxes page
2. ignore checkbox 1
3. select checkbox 2

## Expected Result

Checkbox 1: unchecked
Checkbox 2: unchecked

## Actual Result

Checkbox 1: unchecked
Checkbox 2: unchecked

## Status

pass
