# Wesfarmers-dcf-valuation
Wesfarmers (WES.AX) equity valuation in Excel. Builds a 5-year pro-forma income statement and balance sheet, forecasts revenue with macro regression, estimates beta, and values the company using FCFE and FCFF DCF models.
Wesfarmers (WES.AX) – FCFE & FCFF Valuation

An Excel-based valuation of Wesfarmers Ltd, the Australian conglomerate behind Bunnings, Kmart and Officeworks. The model forecasts the financial statements for FY2026 to FY2030 and values the equity with two discounted cash flow methods.

Model structure

Historical financials
Five years of standardised income statement and balance sheet data (FY2021 to FY2025), in AUD millions.
Revenue forecast
Line items projected as an average percentage of revenue
Total revenue forecast with OLS regression (R² = 0.90)
Macro cross-check that regresses real revenue on Australian real GDP and population growth (1995 to 2025), with 2.5% inflation applied
Pro-forma statements
Income statement and balance sheet forecast for FY2026 to FY2030. Depreciation is linked to prior-year PP&E, and cash is the balancing plug.
Dividend policy
Historical payout ratio averaged 88.2% (retention 11.8%) and applied to forecast earnings.
Beta estimation
76 monthly returns of WES against the ASX 200 (Jan 2020 to Jun 2026)
Raw levered beta: 0.99 (R² = 0.56, t-stat = 9.76)
Unlevered with Hamada, then relevered each year as the forecast D/E changes
Free Cash Flow to Equity (FCFE)
FCFE = Net Income + D&A − ΔWorking Capital − Capex + Net Borrowing
Cost of equity: about 9.5% (CAPM, risk-free rate 2.71%, MRP 7.73%)
Terminal growth: 1.25%
Value per share: $38.06
Free Cash Flow to the Firm (FCFF)
FCFF = FCFE + Interest × (1 − T) − Net Borrowing
WACC: about 5.8%, recalculated each year
Value per share: $62.06
Model integrity checks
Duality checks for both FCFE and FCFF, comparing the cash-flow build-up with the balance-sheet approach
FCFE-to-FCFF reconciliation, where every difference comes out at zero
Every component is formula-linked to the pro-forma statements, with no hardcoded values

Results

FCFE value per share: $38.06
FCFF value per share: $62.06
Market price (1 Jul 2025): $73.47
Recommendation: SELL

Both methods put Wesfarmers below its market price. The market seems to be pricing in more growth and a stronger brand premium than a 1.25% terminal growth rate allows.

Data sources
LSEG/Refinitiv (financial statements and prices), ABS (real GDP, CPI and population), RBA (bond yields).

Tools
Microsoft Excel (Data Analysis ToolPak for the regressions)
