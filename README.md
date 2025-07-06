# DCF Valuation Model – Infosys Ltd

This project performs a Discounted Cash Flow (DCF) valuation of Infosys Limited using historical financial data and forecast assumptions.

## Overview

The DCF model estimates the intrinsic value of Infosys by:

- Using historical financial data (FY21–FY25) including revenue, EBIT, net income, depreciation, CapEx, net working capital changes, and net debt.
- Forecasting future financials (FY26–FY30) based on growth, margins, tax rate, and capital expenditure assumptions.
- Calculating Free Cash Flows (FCF) from forecasted figures.
- Discounting FCFs to present value using a Weighted Average Cost of Capital (WACC) of 8%.
- Computing terminal value and adding it to the enterprise value.
- Adjusting for net debt to find equity value.
- Determining intrinsic value per share based on outstanding shares.

## Final Valuation Summary

| Metric                    | Value (₹ Cr)        |
|---------------------------|---------------------|
| Discounted Terminal Value | 304,334             |
| Enterprise Value          | 405,012             |
| Equity Value              | 405,012 (net debt = 0) |
| Intrinsic Value per Share | ₹957.12             |

## Project Files

- `dcf_model.py` — Python script implementing the DCF valuation  
- `infosys_data.csv` — Historical financial data used in the model  
- `dcf_documentation.tex` — LaTeX report detailing the valuation process and results

## How to Use

1. Review and adjust assumptions in `dcf_model.py` as needed.
2. Run the Python script to generate valuation outputs.
3. Refer to `dcf_documentation.tex` for the full report and methodology.

## Conclusion

This DCF valuation provides a data-driven estimate of Infosys’s intrinsic value, useful for investment analysis and decision making.

---

*Feel free to explore and modify the model according to your needs.*
