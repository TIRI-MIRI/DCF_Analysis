# DCF Valuation Model

This project implements a Discounted Cash Flow (DCF) valuation model to estimate the intrinsic value of any publicly listed company using historical financial data and customizable forecast assumptions.

## Overview

- Uses historical financial data such as revenue, EBIT, net income, depreciation, capital expenditure, net working capital changes, and net debt.
- Forecasts future financial performance (typically 5 years) based on user-defined assumptions.
- Calculates Free Cash Flows (FCF) for each forecast year.
- Discounts FCFs to present value using a specified Weighted Average Cost of Capital (WACC).
- Computes terminal value at the end of the forecast period and discounts it.
- Adds discounted FCFs and terminal value to compute Enterprise Value.
- Adjusts for net debt to estimate Equity Value.
- Divides Equity Value by the number of outstanding shares to calculate the intrinsic value per share.

## Final Valuation Summary

- Discounted Terminal Value  
- Enterprise Value  
- Equity Value  
- Intrinsic Value per Share  

## Project Files

- `dcf_model.py` – Python script implementing the DCF valuation logic.
- `financial_data.csv` – CSV file containing historical financial data.
- `dcf_documentation.tex` – LaTeX file describing methodology and valuation results.

## How to Use

1. Replace `financial_data.csv` with the target company’s historical financials.
2. Adjust assumptions in `dcf_model.py`, including:
   - Revenue growth rates
   - Operating margins (EBIT)
   - Tax rate
   - Depreciation and CapEx
   - Net working capital assumptions
   - Terminal growth rate
   - WACC
   - Number of outstanding shares
3. Run the script:
