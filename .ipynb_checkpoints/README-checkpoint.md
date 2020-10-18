# <center> **FINANCIAL PLANNER - SAVING & RETIREMENT**

### This Financial planner focuses to create two financial analysis tools.
1. personal finance planner to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund
2. Retirement planning tool using monte carlo simulation tool kit composed of stocks and bonds and run Monte Carlo simulations to project the portfolio performance at various time periods and investment levels

The tools are developed in Python using Jupyter lab. The libraries/packges imported to Pandas are:
    
    1. os
    2. requests
    3. pandas
    4. dotenv
    5. alpaca_trade_api
    6. MCForecastTools (included)
    7. matplotlib
    
### Resources
This project will utilize two APIs:
* The **Alpaca Markets API** will be used to pull historical stocks and bonds information.    
* The **Alternative Free Crypto API** will be used to retrieve Bitcoin and Ethereum prices.

The documentation for these APIs can be found via the following links:
* [Free Crypto API Documentation](https://alternative.me/crypto/api/)
* [AlpacaDOCS](https://alpaca.markets/docs/)
    
    
### Part 1 - Personal Finance Planner
Collect Crypto Prices Using the `requests` Library
Parse the API JSON response to select only the crypto prices using specific identifiers   
    
To develop the personal finance planner prototype, you should take into account the following assumptions:
1. units of crypto assets: `1.2` BTC and `5.3` ETH
2. units of shares in stocks and bonds: `50` SPY (stocks) and `200` AGG (bonds)
3. `monthly_income` and set its value to `12000` to perform saving analysis  

   
### Part 2 - Retirement Planning
the Alpaca API is used to fetch historical closing prices for a retirement portfolio and the MCForecastTools toolkit to create Monte Carlo simulations to project the portfolio performance.
    
Configure and execute a Monte Carlo Simulation 
Fetch the summary statistics from the Monte Carlo simulation results.
Plot the simulation results and the probability distribution/confidence intervals.
calculate the expected portfolio return in dollars at the `95%` lower and upper confidence intervals.     
   
To develop the Retirement planner prototype, you should take into account the following assumptions: 

1. an initial investment of `$20,000`
2. No. of simulations 500
3. No.of days in a trading year 252
4. Weights are  40/60 portfolio for the tickers SPY and AGG
