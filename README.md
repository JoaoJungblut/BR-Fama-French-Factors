# Fama-French_Factors

Factor-Based Portfolio Construction is a strategy employed in finance and investment to create diversified portfolios based on specific factors or characteristics of individual stocks. This approach aids investors in identifying stocks with desirable attributes and forming portfolios with the potential to outperform the market. The process involves selecting and classifying stocks based on particular factors, combining them into portfolios, and periodically rebalancing to maintain the desired characteristics.The data was downloaded from **Economatica**.

## Factors

1. **Risk Premium (R_mkt - R_f):** The risk premium factor represents the excess return of the overall market (R_mkt) over the risk-free rate (R_f). It measures the compensation investors require for taking on the risk associated with investing in stocks.

2. **Small Minus Big (SMB):** SMB is a factor that captures the difference in returns between small-cap and large-cap stocks. It assesses whether smaller companies tend to outperform their larger counterparts.

3. **High Minus Low (HML):** HML factor evaluates the performance disparity between high book-to-market (value) and low book-to-market (growth) stocks. It helps in identifying the impact of a company's financial position on returns.

4. **Robust Minus Weak (RMW):** RMW factor measures the difference in returns between companies with strong operating profitability (robust) and those with weak operating profitability. It highlights the influence of profitability on stock performance.

5. **Conservative Minus Aggressive (CMA):** The CMA factor assesses the contrast in returns between conservative companies and aggressive companies. It reflects how a company's investment decisions impact its performance.

6. **Winner Minus Losers (WML):** WML factor compares the returns of winning stocks to those of losing stocks. It reveals the impact of a company's recent performance on its future returns.

7. **Reversal Factor (Return to Mean):** The Reversal factor evaluates the returns based on a stock's momentum and its tendency to revert to the mean. It measures the effects of price trends on future performance.

## Portfolios

Factor-Based Portfolios are constructed by grouping stocks based on various factors. These portfolios are typically categorized by the following factors:

### Size and Book-to-Market

- **Small (Value / Neutral / Growth):** Stocks are classified as small or big, and within these categories, they are further divided based on their book-to-market ratios, distinguishing between value, neutral, and growth stocks.

- **Big (Value / Neutral / Growth):** Large-cap stocks are categorized into value, neutral, and growth based on book-to-market ratios.

### Size and Operating Profitability

- **Small (Robust / Neutral / Weak):** Small-cap stocks are categorized into robust, neutral, and weak based on operating profitability.

- **Big (Robust / Neutral / Weak):** Large-cap stocks are categorized into robust, neutral, and weak based on operating profitability.

### Size and Investment

- **Small (Conservative / Neutral / Aggressive):** Small-cap stocks are categorized into conservative, neutral, and aggressive based on their investment returns.

- **Big (Conservative / Neutral / Aggressive):** Large-cap stocks are categorized into conservative, neutral, and aggressive based on their investment returns.

### Size and Momentum

- **Small (High / Low):** Small-cap stocks are grouped based on high and low momentum.

- **Big (High / Low):** Large-cap stocks are categorized into high and low momentum stocks.

### Size and Reversal

- **Small (High / Low):** Small-cap stocks are categorized into high and low reversal stocks.

- **Big (High / Low):** Large-cap stocks are grouped into high and low reversal stocks.

## Company Size

In Factor-Based Portfolio Construction, company size is typically categorized into "Small" and "Big" based on their market capitalization (ME). Small companies are those with market capitalization below the median, while big companies have market capitalization above the median.

## Indicators

Several key indicators play a vital role in the classification and construction of factor-based portfolios:

- **Book-to-Market (B/M):** The B/M ratio is calculated as the ratio of book equity (BV) to market equity (MV) and helps categorize stocks into value, neutral, and growth.

- **Operating Profitability (OP):** OP is measured as the ratio of Operating Profitability to book equity (BV) and classifies stocks into robust, neutral, or weak.

- **Investment (INV):** The investment factor is determined based on the return on assets (ROA) and categorizes stocks into conservative, neutral, or aggressive.

- **Momentum:** Momentum is calculated as the percentage change in a stock's price over a specified period, typically 250 days ago. This factor helps categorize stocks as high or low momentum.

## Building the Factors

The process of building factor-based portfolios involves the following steps:

1. Select companies with Market Value greater than 0.
2. Calculate the median Market Value and classify companies as small or big.
3. Classify companies based on the indicators (B/M, OP, INV) into growth, neutral, or value (or robust, neutral, weak, and conservative, neutral, aggressive).
4. Calculate the factor values (e.g., SMB, HML, RMW, CMA, WML, ST_rev) based on the factor definitions and the classifications of stocks into different categories.
5. Rebalance portfolios at the end of June to maintain the desired factor characteristics.

Factor-Based Portfolio Construction is a sophisticated approach to investing, leveraging quantitative and statistical methods to design portfolios that aim to capture specific risk and return factors. It provides investors with a systematic way to structure their investments based on factors that have historically been associated with higher returns.
