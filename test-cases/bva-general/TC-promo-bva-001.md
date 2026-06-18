# Test Case: TC-promo-bva-001

**Title:** `TC-promo-bva-001.md`: Too low value
**Feature or component under test:** Promo code discount field
**Design technique used:** boundary value analysis
**Linked charter or requirement:** A promo code discount field accepts a whole-number percentage from 10 to 75 inclusive. Values below 10 or above 75 are rejected.

## Preconditions

Promo code field must be empty and actionable. Assuming there is a 'confirm' button on the page.

## Test Data

### Partitions

The minimum boundary is 9/10, dividing the too low and valid partitions.
The maximum boundary is 75/76, dividing the valid and too high partitions.

Note: boundary values highlighted below

Too low: max(8,**9**,10)
Valid: min(9,**10**,11) / max(74,**75**,76)
Too high: min(75,**76**,77)

The too low and min-valid partitions catch a missing `=` in the low-end comparison.
The too high and max-valid partitions catch a missing `=` in the high-end comparison.

Chosen partition value: min-valid: (9,**10**,11)

## Steps

1. Load promo code discount field
2. Attempt discount code: 9
3. Clear discount field
4. Attempt discount code: 10
5. Clear discount field
6. Attempt discount code: 11

## Expected Result

9: rejected
10: accepted
11: accepted

## Actual Result

Hypothetical scenario not based on a real DOM. Not possible to get an actual result. If there were a missing `=` in the low end comparison, 10 would be erroneously rejected.

## Status

not run
