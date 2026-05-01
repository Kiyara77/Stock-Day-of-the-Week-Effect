# Stock-Day-of-the-Week-Effect

A data analysis project investigating the **day-of-the-week effect** in Chinese stock market returns, using the **Shanghai Composite Index (SSE)** and **Shanghai Pudong Development Bank (SPDB)** as case studies.

## 📌 Overview

The "day-of-the-week effect" refers to the empirical observation that stock returns may systematically differ depending on the day of the week—e.g., lower returns on Mondays or higher volatility on Fridays.  
This project analyzes daily price data to visualize and explore whether such patterns exist in the A-share market.

## 📊 Data Source

- Excel file: `D://24108108Hong.xlsx` (Sheet: `Sheet1`)
- Columns used:
  - `Date`: Trading date (formatted as MM/DD/YY)
  - `上证指数`: Shanghai Composite Index closing price
  - `浦发银行`: SPDB stock closing price

> Note: The dataset is assumed to contain only trading days (no weekends/holidays).

## 🛠️ Methodology

1. **Data Cleaning**
   - Extract relevant columns (`Date`, `SSE Index`, `SPDB`)
   - Convert `Date` to `datetime` format
   - Remove missing values

2. **Feature Engineering**
   - Compute daily simple returns
   - Assign weekday numbers: Monday = 1, ..., Friday = 5

3. **Visualization**
   - Reshape data to long format
   - Plot **boxplots of daily returns by weekday** for both assets using `seaborn`

## 📈 Key Output

- Shows distribution (median, IQR, outliers) of returns across weekdays
- Horizontal dashed line at return = 0 for reference
- Compares market index (SSE) vs. individual stock (SPDB)

## ▶️ How to Run

1. Place the data file at the specified path or update the file path in the script.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
