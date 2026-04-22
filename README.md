# Portfolio-Risk-Analysis
Portfolio analytics project using Python to compare investment strategies and quantify risk through volatility, drawdowns, VaR, and CVaR.

## Overview
This project constructs and analyses equity portfolios using Python, with a focus on both performance and downside risk.

Two portfolio strategies are compared:
- Equal-weight portfolio  
- Momentum-based portfolio  

The analysis evaluates return, volatility, and risk using industry-standard metrics such as Sharpe Ratio, Maximum Drawdown, Value at Risk (VaR), and Conditional Value at Risk (CVaR).

## Objective
The goal of this project is to:
- Compare portfolio performance across strategies  
- Quantify risk exposure using statistical measures  
- Analyse behaviour during adverse market conditions  

## Data
- Source: Yahoo Finance  
- Frequency: Monthly data (resampled from daily prices)  
- Period: 2015 – 2024  
- Assets:
  - Apple (AAPL)  
  - Microsoft (MSFT)  
  - Tesla (TSLA)  
  - Amazon (AMZN)  
  - NVIDIA (NVDA)  

## Methodology

### 1. Data Preparation
- Downloaded daily adjusted prices  
- Converted to monthly data  
- Calculated percentage returns  

### 2. Portfolio Construction
- Equal Weight Portfolio: 20% allocation to each stock  
- Momentum Portfolio: Top 2 stocks based on past 3-month returns (monthly rebalancing)  

### 3. Performance Metrics
- Annual Return  
- Annual Volatility  
- Sharpe Ratio  
- Maximum Drawdown  

### 4. Risk Metrics
- Value at Risk (VaR)  
- Conditional Value at Risk (CVaR)  

## Results

### Final Summary Table

| Portfolio | Annual Return | Volatility | Sharpe Ratio | Max Drawdown | VaR (95%) | CVaR (95%) |
|----------|--------------|------------|--------------|--------------|-----------|------------|
| Equal Weight | 49.44% | 29.15% | 1.33 | -45.13% | -10.66% | -13.87% |
| Momentum | 66.61% | 38.49% | 1.30 | -54.67% | -12.10% | -13.73% |

## Visualisations

### Cumulative Returns
Cumulative Returns

### Drawdown Comparison
Drawdown

## Key Insights

- The momentum strategy delivered higher absolute returns  
- The equal-weight portfolio achieved slightly better risk-adjusted performance (higher Sharpe ratio)  
- Momentum exhibited higher volatility and deeper drawdowns  
- VaR indicates higher downside risk for the momentum portfolio  
- CVaR suggests similar extreme loss severity across both strategies  

## Conclusion
The analysis highlights a clear trade-off between return and risk. While the momentum strategy enhances returns, it also increases exposure to volatility and downside risk. The equal-weight portfolio provides more stable performance on a risk-adjusted basis.

## Limitations
- Limited to 5 large-cap US stocks  
- Simplified transaction cost assumption  
- No macroeconomic or external factors included  

## Future Improvements
- Expand asset universe for diversification  
- Incorporate dynamic transaction costs  
- Add additional strategies (low volatility, mean reversion)  
- Integrate machine learning-based allocation  

## Tools Used
- Python (Pandas, NumPy, Matplotlib)  
- yfinance  
