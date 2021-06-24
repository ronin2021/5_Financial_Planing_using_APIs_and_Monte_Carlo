# Finacial Planing and porfolio forcasting using API Data Extraction and Monte Carlo Simulation to forward forcast performance

## Outline

Individual's portfolio is assumed to have some collection of crypto currencies (non-traditional) and shares and bonds (traditional). Entire code is written in Python. A number of libraries were used as illustrated in the code. Data extraction (closing for crypto, stocks, and bonds) was via given API. Subsequently a Monte Carlo simulation was used for forcasting the traditional portion of the portfolio with various weights (in part 2 optional). A .env file is required with API key and secret key for Alpaca API where the data extraction is coming from.   

### Part 1. Savings and Emergency Fund
  1. A number of crypto, bond, and stock assets are provided for an individuals portfolio 
  2. URL of the "alternative.me" was used to extract her respective crypto holdings data.  
  3. These were used to extract current closing price.
  4. Then calculate the crypto assets collective market value
  5. Designated bond and stock data were extracted from Alpaca API providing current closing price. 
  6. Then calculate the both bond and stock assets collective market value.
  7. total asset value was shown using pie chart.
  8. Individuals monthly salary was given and it was assesd if she has three months of salary equivalent total assets for an emmergency fund.

### Part 2. Retirement Planing

  1. For the bond and and stock assets 5 years worth of financial data including the closing price was extracted. 
  2. Date formatted dat were inspected 
  3. 40% to 60% bond to stock weighted portfolio was passed. 
  4. A 30-year Monte-Carlo Simulation was run this weighted portfolio with 500 iterations with 30 * 252 = 7560 trading days.  
  5. Each simulation was plotted for cumulative gains.
  6. Collective distribution of gains were plotted.
  7. Retirement projection with upper and lower bound at 95% confidence interval was obtained with other relevant statistical values.
  8. For an initial principle of $20,000 and then a principle of $30,000 (50% increase from the previous) the 95% bounds were calculated provide range of forcaste. 

### Optional Early Retirement Planing

  1. Previously extracted bond and and stock assets 5 years worth of financial data including the closing price was used for the simultions. 
  2. 10% to 90% bond to stock weighted portfolio was passed to account for needed high return typically via stocks.  
  3. A 5-year Monte-Carlo Simulation was run this weighted portfolio with 1000 iterations with 5 * 252 = 1260 trading days.  
  4. Each simulation was plotted for cumulative gains.
  5. Collective distribution of gains were plotted.
  6. Retirement projection with upper and lower bound at 95% confidence interval was obtained with other relevant statistical values.
  7. For an initial principle of $80,000 (to compensate for early retirement likely a higher principle is needed) the 95% bounds were calculated provide range of forcaste.
  8. 20% to 80% bond to stock weighted portfolio was passed to account for needed high return typically via stocks. But in this senario to reduce the risk stock fraction was    reduced as the projected time was increased to 10-yeras.  
  9. A 10-year Monte-Carlo Simulation was run this weighted portfolio with 1000 iterations with 10 * 252 = 2520 trading days.  
  10. Each simulation was plotted for cumulative gains.
  11. Collective distribution of gains were plotted.
  12. Retirement projection with upper and lower bound at 95% confidence interval was obtained with other relevant statistical values.
  13. For an initial principle of $60,000 (a reduction due to the increase in projected time to 10-years from the previous value) the 95% bounds were calculated provide range of forcaste.

## Inputs
Read from API and URLs provided and appropriate for the analysis. 

## Outputs
Outputs are given out as mentioned above on the terminal as calculated values, visual plots/graphs/figures, and short sentence derived from results. 

## Remarks
None.
