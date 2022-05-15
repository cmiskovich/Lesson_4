# Lesson_4
# Primary application file

Produce a Jupyter notebook that contains your data preparation, analysis, and visualizations for key risk and return metrics. You should use text and comments to document your findings and answer the question prompts in the instructions. Specifically, this file should contain the following:

A single DataFrame imported from a CSV file that has a DateTimeIndex.

A risk analysis of the assets that the DataFrame contains vs. the S&P 500. This analysis should include risk-return metrics, including the daily returns, standard deviation, Sharpe ratio, and beta.

An evaluation of each asset that uses rolling statistics to track the risk-reward behavior over time.

---

## Technologies

The following Technologies were used to develop this program:

Python 
    Version 3.9.7

Terminal
    Version 2.12.5 (444)

Visual Studio Code
    Version: 1.66.2 (Universal)
    Commit: dfd34e8260c270da74b5c2d86d61aee4b6d56977
    Date: 2022-04-11T07:49:20.994Z
    Electron: 17.2.0
    Chromium: 98.0.4758.109
    Node.js: 16.13.0
    V8: 9.8.177.11-electron.0
    OS: Darwin x64 21.4.0
    
Jupyter Lab 
    Version 3.2.9

---

## General information about analysis.

During the analysis you realize the best funds compared to the S&P 500 are Tiger Global and Berkshire Hathaway.  When you take them on individually you then see that Berkshire Hathaway has less risk reward compared to the S&P 500.  The visualizations and calculations really help reinforce the initial data of returns and cumulative returns.

---

## Information about datasets

You start the analysis with reading the csv file whale_navs.  The file includes data for the Soros Fund Management, Paulson & Company, Tiger Global Managment, Berkshire Hathaway and the S&P 500.  

whale_navs is a dataset showing the net asset value (NAV) for the 4 funds and the data for S&P 500 index.

daily_returns is the percent change in the previous day's price.

daily_returns_four this is the dataset without the S&P 500 index data.

daily_returns_21 is the 21 day rolling window for daily_returns.

daily_returns_21_four is the 21 day rolling window for daily_returns excluding S&P 500 index.

daily_returns_60 is the 60 day rolling window for daily_returns variances for all funds and S&P 500 index.

daily_returns_60_sp500 is the 60 day rolling window for daily_returns variances for only the S&P 500 index.

cumulative_return is the cumulative returns for the entire time frame.

volatility is the standard deviation for daily returns.

volatility_annual using the square root of the standard deviation and 252 trading days we are able to get the annual standard deviation.

avg_annual is the average annualize average return data.

sharpe_ratios calculates the sharpe ratio (avg_annual / daily_returns.std() * np.sqrt(252) for each of the funds and S&P 500 index.

daily_returns_60_cov_tiger covaraiance for Tiger Global Management.

daily_returns_60_cov_bh covariance for Berkshire Hathaway.

beta_tiger beta for Tiger Global Management.

beta_bh beta for Berkshire Hathaway.

beta_tiger_avg used to calculate the average value of the 60 day rolling beta.

beta_bh_ avg used to calculate the average value of the 60 day rolling beta.


---

## Libraries used in analysis

Pandas

Path

Seaborn

Numpy

%matplotlib

---

## Contributors


**Chris Miskovich**

Contact Information:

Email: cmiskovich@verizon.net

[LinkedIn](https://www.linkedin.com/in/christopher-miskovich-9a61b0234/) 

---

## License

[MIT](/license.txt)
