# Trading Strategy Analysis Dashboard

Comprehensive interactive dashboard for in-depth trading strategy performance analysis, risk assessment, and statistical evaluation using Python and Jupyter widgets.

## Features

- **Interactive Visualizations**: Dynamic equity curves, drawdown analysis, and profit/loss distributions
- **Multi-dimensional Trade Analysis**: Performance breakdown by hour, direction, exit reasons, weekdays, and months
- **Comprehensive Risk Metrics**: Value at Risk (VaR), Expected Shortfall, Sharpe/Sortino/Calmar ratios, Ulcer Index
- **Statistical Analysis**: Distribution properties, autocorrelation, normality tests, win/loss streak analysis
- **Monte Carlo Simulations**: Strategy robustness testing with configurable slippage modeling
- **Advanced Analytics**: Kelly Criterion, Expectancy, Win/Loss ratio, rolling statistics
- **Strategy Assessment**: Automated scoring and optimization recommendations

## Technical Architecture
Data Loading → Performance Metrics → Interactive Dashboards → Statistical Analysis → Risk Assessment → Strategy Optimization

## Complete Dashboard Components

### 1. Interactive Visualizations Dashboard
- **Equity Curve**: Dynamic performance chart with date navigation
- **Drawdown Analysis**: Maximum drawdown visualization and recovery periods
- **Profit/Loss Distribution**: Histogram with statistical properties and break-even line
- **Rolling Performance**: Configurable window-based P&L and win rate analysis
- **Customizable Display**: Toggle individual charts on/off for focused analysis

### 2. Trade Analysis Dashboard
- **Temporal Analysis**: Performance by hour of day with 24-hour coverage
- **Directional Analysis**: Long vs. Short trade performance comparison
- **Exit Reason Analysis**: Top N exit reasons with performance metrics
- **Multi-dimensional Metrics**: Profit, win rate, trade count analysis
- **Best Category Focus**: Detailed distribution analysis of top-performing categories

### 3. Advanced Trade Analytics Dashboard
- **Extended Time Analysis**: Weekday and monthly performance patterns
- **Expectancy Analysis**: Expected value per trade across different categories
- **Comprehensive Filtering**: Multiple analysis dimensions and metric types
- **Interactive Controls**: Dynamic parameter adjustment for real-time insights

### 4. Statistical Analysis Dashboard
- **Distribution Analysis**: Return distribution with normality testing (Jarque-Bera)
- **Statistical Properties**: Skewness, kurtosis, and distribution characteristics
- **Autocorrelation Analysis**: Serial correlation of returns at configurable lags
- **Rolling Statistics**: Dynamic mean, standard deviation, and Sharpe ratio calculations
- **Win/Loss Streak Analysis**: Distribution of consecutive winning and losing streaks
- **Statistical Significance**: T-tests and confidence intervals for strategy returns

### 5. Risk Analysis & Monte Carlo Dashboard
- **Value at Risk (VaR)**: Historical and parametric VaR at multiple confidence levels (90%, 95%, 99%)
- **Expected Shortfall**: Tail risk assessment beyond VaR calculations
- **Risk-Return Distribution**: Combined visualization of returns and risk metrics
- **Monte Carlo Simulations**: Equity path modeling with configurable slippage impact
- **Probability Distributions**: Success probability and worst-case scenario analysis
- **Comprehensive Risk Metrics**: Sharpe, Sortino, Calmar ratios with confidence intervals

### 6. Comprehensive Strategy Assessment Dashboard
- **Multi-factor Scoring System**: 6-point evaluation based on risk tolerance profiles
- **Risk-Adjusted Rating**: Automated strategy classification (Excellent/Very Good/Good/Needs Improvement)
- **Kelly Criterion**: Optimal position sizing calculations and recommendations
- **Strategy Expectancy**: Expected value per trade analysis and optimization guidance
- **Performance Benchmarking**: Against customizable risk-adjusted thresholds
- **Actionable Recommendations**: Specific, context-aware optimization suggestions

## Complete Analysis Metrics

### Core Performance Metrics
- **Total Return**: Percentage and absolute profit/loss
- **Net Profit**: Final equity minus initial capital
- **Profit Factor**: Gross profit divided by gross loss
- **Win Rate**: Percentage of profitable trades
- **Max Drawdown**: Maximum peak-to-trough decline
- **Sharpe Ratio**: Risk-adjusted returns annualized

### Advanced Performance Metrics
- **Expectancy**: Expected value per trade calculated from win rate and average win/loss
- **Win/Loss Ratio**: Average winning trade divided by average losing trade
- **Kelly Fraction**: Optimal position size based on win probability and payoff ratio
- **Largest Win/Loss**: Maximum individual trade profit and loss
- **Average Trade**: Mean profit per trade across all transactions

### Risk Management Metrics
- **Value at Risk (VaR)**: Maximum expected loss at given confidence levels
- **Expected Shortfall**: Average loss beyond VaR threshold
- **Sortino Ratio**: Downside risk-adjusted returns
- **Calmar Ratio**: Return relative to maximum drawdown
- **Ulcer Index**: Measure of portfolio drawdown risk
- **95% VaR & 99% VaR**: Multiple confidence level risk assessment

### Statistical Metrics
- **Skewness**: Measure of return distribution asymmetry
- **Kurtosis**: Measure of distribution tail thickness
- **Jarque-Bera Test**: Normality test with p-value significance
- **Autocorrelation**: Serial correlation analysis at multiple lags
- **T-test Significance**: Statistical significance of strategy returns
- **Rolling Statistics**: Time-varying mean, volatility, and risk-adjusted ratios

### Trade Analysis Metrics
- **Hourly Performance**: Profitability patterns throughout trading day
- **Directional Performance**: Long vs. short trade effectiveness
- **Exit Reason Analysis**: Performance attribution by trade closure原因
- **Temporal Patterns**: Weekly and monthly seasonality analysis
- **Trade Duration**: Impact of holding period on profitability
- **Streak Analysis**: Consecutive winning and losing trade patterns

### Monte Carlo Simulation Metrics
- **Probability of Profit**: Likelihood of ending with positive equity
- **Average Final Equity**: Expected ending capital across simulations
- **Worst-Case Scenarios**: 5% VaR from simulation results
- **Best-Case Scenarios**: 95% percentile performance
- **Slippage Impact**: Sensitivity to execution costs and market impact
- **Strategy Robustness**: Consistency across different trade sequences

## Technical Implementation

- **Data Processing**: Pandas for comprehensive time series analysis and data manipulation
- **Visualization**: Matplotlib/Seaborn for statistical charts, distributions, and interactive graphs
- **Interactivity**: IPyWidgets with sliders, dropdowns, and checkboxes for dynamic control
- **Statistical Analysis**: SciPy, Statsmodels for advanced mathematical computations and tests
- **Risk Modeling**: Custom Monte Carlo simulations, bootstrap methods, and statistical testing
- **Performance Analytics**: Comprehensive trading metrics library with risk-adjusted calculations
- **Export Capabilities**: CSV output for further analysis and reporting

## Interactive Controls

- **Rolling Window Size**: Adjustable from 5 to 100 trades for performance smoothing
- **Confidence Levels**: VaR calculations from 90% to 99% confidence
- **Slippage Modeling**: Configurable from 0% to 5% maximum slippage
- **Simulation Count**: Monte Carlo runs from 100 to 2000 simulations
- **Risk Tolerance**: Low/Medium/High profiles for strategy assessment
- **Analysis Dimensions**: Multiple categorization options (hour, direction, exit reason, etc.)
- **Metric Selection**: Profit, win rate, count, expectancy across different views

# License
This project is licensed under the MIT License - see the LICENSE file for details.

# Disclaimer
This trading analysis tool is for educational and research purposes only. Always conduct thorough backtesting, forward testing, and risk assessment before implementing any trading strategy. Past performance does not guarantee future results. Use at your own risk. Professional financial advice is recommended for live trading.
