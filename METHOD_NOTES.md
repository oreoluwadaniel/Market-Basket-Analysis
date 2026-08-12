# Method Notes

## Association rules

The analysis uses transaction-level baskets to identify products that appear together.

The three core measures are:

- **Support:** how often the combination appears in all transactions.
- **Confidence:** how often the second product appears when the first product appears.
- **Lift:** how much more often the pair occurs than would be expected from the products' individual frequencies.

Lift is useful for ranking relationships, but it does not prove that one product causes the other purchase.

## Business use

A strong rule can be considered for:

- bundle testing
- cross-sell placement
- related-product recommendations
- promotion planning

A production recommendation should be tested against a control group and judged on incremental revenue, margin, and average order value.

## Portfolio position

This is an earlier retail case study. The current flagship retail repository is `everdale-retail-analytics`, which adds ETL, data-quality controls, customer analysis, profitability, and forecasting.
