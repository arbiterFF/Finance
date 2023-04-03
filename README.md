# Modern Portfolio Theory Optimizer

This project is a Python implementation of Modern Portfolio Theory (MPT) to optimize a portfolio of stocks using historical data. The goal is to maximize the Sharpe ratio, which represents the risk-adjusted return of the portfolio.

## Features

- Fetch stock price data using `yfinance` library
- Calculate daily returns, mean returns, and covariance matrix
- Optimize the portfolio by maximizing the Sharpe ratio
- Display individual stock performance, optimized portfolio weights, and overall portfolio performance

## Dependencies

- numpy
- pandas
- yfinance
- datetime
- scipy

To install the dependencies, run:


pip install numpy pandas yfinance datetime scipy


## Usage

1. Define the stocks in your portfolio by modifying the `stocks` list:


stocks = ['BHP.AX', 'BXB.AX', 'CSL.AX', 'MQG.AX', 'NAB.AX', 'RIO.AX', 'RMD.AX', 'SHL.AX', 'TCL.AX', 'WDS.AX', 'WTC.AX', 'TNE.AX', 'TLX.AX', 'APA.AX', 'TLS.AX']


2. Set the time period for the analysis by modifying the `start_date` and `end_date` variables:


end_date = datetime.datetime.now()
start_date = end_date - datetime.timedelta(days=180)


3. Run the script to fetch stock price data, calculate returns and optimize the portfolio:


python mpt_optimizer.py


4. The script will display the individual stock performance, optimized portfolio weights, and overall portfolio performance, including expected return, volatility, and Sharpe ratio.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
