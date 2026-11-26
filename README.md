# S&P 500 Stock Prices Analysis (2014--2017)

## Project Overview

This project explores historical stock market data covering the period
from January 2014 to December 2017. The analysis was conducted using
Python to examine stock prices, daily returns, trading volume and
volatility across 505 stock symbols.

The project focuses on understanding historical market behaviour,
comparing individual stock performance and presenting important findings
through interactive visualisations.

## Project Objectives

-   Understand the structure and quality of the stock prices dataset.
-   Clean and prepare the data for analysis.
-   Explore historical stock price movements.
-   Calculate daily price changes and percentage returns.
-   Analyse trading volume and stock volatility.
-   Compare selected stocks over the available period.
-   Develop interactive dashboards to communicate findings.

## Dataset Description

The dataset contains historical stock trading records from 2014 to 2017.

**Dataset features:**

  Column     Description
  ---------- ---------------------------------------
  `symbol`   Stock ticker symbol
  `date`     Trading date
  `open`     Opening stock price
  `high`     Highest price recorded during the day
  `low`      Lowest price recorded during the day
  `close`    Closing stock price
  `volume`   Number of shares traded

**Dataset summary:** - Original records: 497,472 - Cleaned records:
497,461 - Stock symbols: 505 - Date range: 2014-01-02 to 2017-12-29 -
Missing values identified: 27 - Exact duplicate rows: None identified

## Tools and Libraries

The project was completed using:

-   **Python** -- Main programming language.
-   **Pandas** -- Data cleaning, manipulation and analysis.
-   **NumPy** -- Numerical calculations.
-   **Matplotlib** -- Exploratory data visualisation.
-   **Plotly Express** -- Interactive charts and dashboards.
-   **Plotly Graph Objects** -- KPI indicators and dashboard elements.
-   **Jupyter Notebook** -- Development and documentation environment.

## Project Workflow

### 1. Data Understanding

The dataset was inspected to understand its dimensions, columns, data
types, date range, stock symbols and general statistical properties.

### 2. Data Cleaning and Preparation

The preparation process included: - Converting the date column into
datetime format. - Sorting records by stock symbol and date. - Checking
missing values and duplicate records. - Investigating zero-volume
observations. - Identifying unusual stock price relationships. -
Removing 11 records with missing required price values.

Unusual price observations were investigated and flagged rather than
automatically removed.

### 3. Feature Engineering

Additional analytical columns were created: - Year - Month - Quarter -
Daily price change - Daily percentage return - Trading range - 7-day
moving average - 30-day moving average - Price anomaly indicator

Calculations involving previous prices and moving averages were
performed separately for each stock.

### 4. Exploratory Data Analysis

The analysis examined: - Average closing prices by year. - Monthly stock
price movements. - Highest and lowest average closing prices by stock. -
Average daily returns. - Return distributions and volatility. - Average
and total trading volume.

### 5. Interactive Dashboard Development

Four dashboard sections were developed using Plotly:

**Dashboard 1 -- Market Overview** - Total stock symbols. - Trading
records. - Average closing price. - Years covered. - Average closing
price by year.

**Dashboard 2 -- Stock Price Performance** - Closing price trends for
selected stocks. - Opening, highest and lowest price movements for a
selected stock.

**Dashboard 3 -- Returns and Volatility** - Daily percentage returns. -
Average daily returns by stock. - Daily return distribution. -
Historical volatility.

**Dashboard 4 -- Trading Volume Analysis** - Trading volume trends. -
Average trading volume by stock. - Highest and lowest trading volume
observations. - Trading volume versus daily price change.

The dashboards include interactive Plotly charts and date range sliders
where applicable.

## Key Findings

-   The average closing price across the full dataset increased from
    approximately \$76.97 in 2014 to \$98.80 in 2017.
-   NVDA recorded the highest average daily return among the stocks
    analysed.
-   CHK recorded the highest historical return volatility.
-   PCLN had the highest average closing price, while AMD had the
    lowest.
-   BAC recorded the highest average trading volume.
-   Among the five selected stocks, AMD showed the strongest relative
    price growth when comparing normalised closing prices.

These findings describe the historical observations in the dataset and
are not investment recommendations.

## Dashboard Stock Selection

The stock comparison dashboard uses five selected stocks:

-   BAC -- Bank of America
-   AAPL -- Apple
-   GE -- General Electric
-   AMD -- Advanced Micro Devices
-   F -- Ford Motor Company

The selected stocks were used to compare price performance, returns and
trading activity.

## Validation and Quality Assurance

The notebook includes validation checks for: - Daily return
calculations. - 7-day moving average calculations. - 30-day moving
average calculations. - Stock selection. - Daily price change
calculations.

All five validation checks returned successful matches.

## Repository Contents

-   `Week_6_S&P500_Analysis.ipynb` -- Jupyter Notebook containing the
    analysis, calculations, visualisations and validation.
-   `README.md` -- Project documentation.
-   `S&P 500 Stock Prices 2014-2017.csv` -- Original dataset, if
    included in the repository.

## How to Run the Project

1.  Clone or download this repository.

2.  Install the required Python libraries:

    ``` bash
    pip install pandas numpy matplotlib plotly jupyter
    ```

3.  Place the CSV dataset in an accessible folder.

4.  Open the notebook using Jupyter Notebook or JupyterLab.

5.  Update the CSV file path in the data-loading cell to match your
    local location.

6.  Run the notebook cells in order.

## Conclusion

This project demonstrates the use of Python for practical data analysis,
from data inspection and cleaning to exploratory analysis, feature
engineering, interactive visualisation and validation.

The analysis provides insights into historical stock price behaviour,
daily returns, trading activity and volatility across the available
stock records.
