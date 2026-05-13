# Minara demo strategies

Trading strategies written in pine-runtime, Minara Strategy Studio's TypeScript DSL. Paste any file into Strategy Studio and run your own backtest.

## Strategies

| Asset | Backtest timeframe | Indicators | File |
|---|---|---|---|
| MU (Micron) | 4h | EMA, RSI, MACD | [MU-1600%.txt](MU-1600%25.txt) |
| AMD | 4h | EMA fast/slow, RSI, MACD, ATR | [AMD-65%.txt](AMD-65%25.txt) |

The percentage in each filename is the headline return from the original 4h backtest. Re-run with your own date range, fees, and leverage before relying on it.

## MU Long Momentum

Long only. Three-factor momentum alignment: price above EMA(20), RSI(14) above 50, and MACD line above signal, with at least one of those three freshly triggered on the current bar.

- Stop loss: 2% below entry
- Take profit: 5% above entry
- Trailing stop: activates at +3%, offset 1.5%
- Position sizing: 100% of equity × leverage (aggressive)
- Pyramiding: 1

## AMD Momentum Trend

Long and short. Trend filter on EMA(20) vs EMA(50), entry on RSI cross of 55 (long) or 45 (short) plus MACD confirmation. Stops and targets are sized in ATR units, so risk per trade scales with current volatility.

- Stop loss: 1.5× ATR(14) from entry
- Take profit: 3.0× ATR from entry
- Trailing stop: 2.0× ATR, armed once price moves +1× ATR in your favor
- Position sizing: 20% margin × leverage
- Pyramiding: 1

## Using a strategy

1. Open Strategy Studio in your Minara account.
2. Create a new strategy and paste the file contents into the Code tab.
3. Set the asset, timeframe to 4h (matches the original backtest), and pick a date range, then run a backtest.
4. Adjust the input parameters from the side panel to fit your assumptions.

## Notes

These are demo strategies for learning the runtime. They are not financial advice, and past backtest performance does not predict future returns.
