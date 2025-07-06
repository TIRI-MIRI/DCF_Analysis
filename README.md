# 💹 DCF Valuation Model – Infosys Ltd

This project presents a comprehensive Discounted Cash Flow (DCF) valuation of Infosys Limited using historical financial data and projected assumptions.

---

## 📌 What is DCF?

Discounted Cash Flow (DCF) is a valuation method used to estimate the value of an investment based on its expected future cash flows. These future cash flows are adjusted (discounted) to reflect their present value.

---

## 🛠️ Project Overview

The following key steps were performed:

- 📊 **Historical Data Input**  
  Revenue, EBIT, Net Income, Depreciation, CapEx, Change in NWC, and Net Debt (FY21–FY25).

- 📈 **Forecasting Future Financials (FY26–FY30)**  
  Assumptions:  
  - Growth Rate (g) = 2%  
  - EBIT Margin = 22.2%  
  - Tax Rate = 26.5%  
  - Depreciation & Amortization = 3% of Revenue  
  - CapEx = 1.7% of Revenue  
  - Change in Net Working Capital = 3% of Revenue

- 🧮 **Free Cash Flow (FCF) Calculation**  
  Calculated by adjusting NOPAT with D&A, CapEx, and changes in NWC, all as percentages of forecasted revenue.

- 💰 **Discounting FCFs**  
  Future free cash flows were discounted using the Weighted Average Cost of Capital (WACC) of 8%.

- ⏳ **Terminal Value Calculation**  
  Terminal value was calculated using the final year free cash flow and discounted back to present value.

- 🏢 **Enterprise & Equity Value**  
  Enterprise value was obtained by summing discounted free cash flows and the discounted terminal value. Equity value was derived by subtracting net debt from enterprise value.

- 📉 **Intrinsic Value per Share**  
  Equity value was divided by the total number of outstanding shares to get the intrinsic value per share.

---

## 📊 Final Output

| Metric                    | Value (₹ Cr)       |
|---------------------------|--------------------|
| Discounted Terminal Value | 304,334            |
| Enterprise Value          | 405,012            |
| Equity Value              | 405,012 (net debt = 0) |
| Intrinsic Value per Share | ₹957.12            |

---

## 🔍 Sensitivity Analysis

A sensitivity table was built by varying:  
- WACC from 7% to 10%  
- Terminal growth rate from 1% to 4%  

This allows us to visualize how intrinsic value fluctuates based on these assumptions.

---

## 📁 Project Files

- `dcf_model.py` – Full Python code for DCF analysis  
- `infosys_data.csv` – Historical financial data  
- `sensitivity_table.csv` – Output table for sensitivity analysis  
- `dcf_documentation.tex` – LaTeX version of the report  

---

## 📝 Conclusion

Based on the assumptions and financials used, the DCF-derived intrinsic value of Infosys is approximately **₹957/share**. This model provides a data-driven foundation to assess whether Infosys is overvalued or undervalued in the current market.
