# Fama-French_Factors-
7 Factors Fama-French Model
# Factor-Based Portfolio Construction

## Factors

- **Risk Premium (R_m - R_f):**
- **Small Minus Big (SMB):**
- **High Minus Low (HML):**
- **Robust Minus Weak (RMW):**
- **Conservative Minus Aggressive (CMA):**
- **Winner Minus Losers (WML):**
- **Reversal Factor (Return to Mean):**

## Portfolios

### Size and Book-to-Market
- **Small (Value / Neutral / Growth):**
- **Big (Value / Neutral / Growth):**

### Size and Operating Profitability
- **Small (Robust / Neutral / Weak):**
- **Big (Robust / Neutral / Weak):**

### Size and Investment
- **Small (Conservative / Neutral / Aggressive):**
- **Big (Conservative / Neutral / Aggressive):**

### Size and Momentum
- **Small (High / Low):**
- **Big (High / Low):**

### Size and Reversal
- **Small (High / Low):**
- **Big (High / Low):**

## Company Size

- Select the top 9 stocks based on market capitalization (ME).
- Small: Stocks below the median market capitalization (ME).
- Big: Stocks above the median market capitalization (ME).

## Indicators

- **Book-to-Market (B/M):** Ratio of book equity (BE) to market equity (ME).
- **Operating Profitability (OP):** Ratio of EBITDA to book equity (BE).
- **Investment (INV):** Return on assets (ROA).
- **Momentum:** (Current Price - Price 250 Days Ago) / Price 250 Days Ago.

## Building the Factors

1. Select companies with ME > 0.
2. Calculate the median ME and classify companies as small or big.
3. Classify companies based on indicators (B/M, OP, INV):
   - 0 - 30% (Growth, Weak, or Conservative)
   - 30 - 70% (Neutral)
   - 70 - 100% (Value, Robust, or Aggressive)
4. Calculate the factors:
   - **SMB:**
     - B/M: 1/3(Small Value + Small Neutral + Small Growth) - 1/3(Big Value + Big Neutral + Big Growth)
     - OP: 1/3(Small Robust + Small Neutral + Small Weak) - 1/3(Big Robust + Big Neutral + Big Growth)
     - INV: 1/3(Small Conservative + Small Neutral + Small Aggressive) - 1/3(Big Conservative + Big Neutral + Big Aggressive)
     - SMB = (1/3) * (SMB_BM + SMB_OP + SMB_INV)
   - **HML:**
     - 1/2(Small Value + Big Value) - 1/2(Small Growth + Big Growth)
   - **RMW:**
     - 1/2(Small Robust + Big Robust) - 1/2(Small Weak + Big Weak)
   - **CMA:**
     - 1/2(Small Conservative + Big Conservative) - 1/2(Small Aggressive + Big Aggressive)
   - **WML:**
     - 1/2(Small High + Big High) - 1/2(Small Low - Big Low)
   - **ST_rev:**
     - 1/2(Small Low + Big Low) - 1/2(Small High + Big High)
5. Rebalance portfolios at the end of June.

This project outlines the construction of factor-based portfolios and provides an overview of the factors and indicators used in the process. Feel free to customize and expand upon this README as needed for your specific project.
