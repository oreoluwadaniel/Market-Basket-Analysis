# Retail Purchase and Basket Analysis

A Python retail analysis using transaction-level purchase data to answer two practical questions: which products are commonly bought together, and when demand changes enough to affect promotions or stock planning.

This is an earlier retail case study in my portfolio. The current flagship retail work is [Everdale Retail Analytics](https://github.com/oreoluwadaniel/everdale-retail-analytics), which covers a broader ETL, data-quality, profitability, customer, and forecasting workflow.

## Business questions

- Which products appear together in the same transaction?
- Which product combinations are strong candidates for bundles or cross-sells?
- Which products show clear seasonal demand?
- When should inventory and promotions be adjusted?
- Which purchase patterns could increase average order value?

## Data

The dataset contains online retail transactions with:

| Field | Purpose |
|---|---|
| Invoice Number | Transaction identifier |
| Stock Code | Product identifier |
| Product Description | Product name |
| Quantity | Units purchased |
| Unit Price | Selling price |
| Customer ID | Customer identifier |
| Country | Customer location |

The data is used for portfolio analysis and does not contain private customer records.

## Method

```text
Transaction data
      |
Data cleaning and validation
      |
Purchase-level analysis
      |
Association rules
      |
Seasonal demand analysis
      |
Business recommendations
```

Association rules are evaluated using measures such as support, confidence, and lift. Seasonal analysis looks at changes in product demand over time.

## Example finding

The analysis found a strong purchasing relationship between products such as:

- WHITE HANGING HEART T-LIGHT HOLDER
- REGENCY CAKESTAND 3 TIER

A relationship like this is useful when deciding whether to test a bundle, cross-sell prompt, or related-product placement. The association itself does not prove that a bundle will increase revenue. That would require a controlled test or a follow-up sales analysis.

## Business use

The analysis can support:

**Cross-selling:** suggest related products during checkout.

**Bundling:** test products that frequently appear in the same basket.

**Promotions:** time campaigns around products with strong seasonal demand.

**Inventory planning:** prepare stock for recurring demand peaks.

## Tools

Python, pandas, mlxtend, association rule mining, exploratory analysis, and data visualization.

## Scope and limitations

This is an analytical case study, not a production recommendation engine. The purchase relationships are observational. They show what appeared together in the dataset, not that one product caused customers to buy another.

A production version would test recommended bundles against a control group and measure incremental revenue, margin, and average order value.

## Contact

Daniel Olatunji

Email: danolatunji25@gmail.com
