# Minara demo strategies

Trading strategies written in pine-runtime, Minara Strategy Studio's TypeScript DSL. Paste any file into Strategy Studio and run your own backtest.

## Strategies

| Asset | Backtest timeframe | Indicators | File |
|---|---|---|---|
| MU (Micron) | 4h | EMA, RSI, MACD | [MU-1600%.txt](MU-1600%25.txt) |
| AMD | 4h | EMA fast/slow, RSI, MACD, ATR | [AMD-65%.txt](AMD-65%25.txt) |
| NVDA | 4h | EMA (9/21/50), RSI, ATR | [NVDA-100%-APY.txt](NVDA-100%25-APY.txt) |
| SMSN (Samsung) | 4h | Donchian, EMA (9/21/50), RSI, ADX, ATR | [SMSN-34%.txt](SMSN-34%25.txt) |
| HYPE | 4h | SuperTrend, RSI, EMA, ADX | [HYPE-175%.txt](HYPE-175%25.txt) |
| ZEC | 4h | SuperTrend, RSI, ATR, volume breakout | [ZEC-228%.txt](ZEC-228%25.txt) |
| CRCL (Circle) | 4h | EMA (9/20/50), RSI, ADX, ATR | [CRCL-125%.txt](CRCL-125%25.txt) |
| MRVL (Marvell) | 4h | EMA (5/15/20), ADX, RSI, ATR trail | [MRVL-152%.txt](MRVL-152%25.txt) |
| ORCL (Oracle) | 4h | MACD, ADX, EMA (20/50), ATR SL/TP | [ORCL-84%.txt](ORCL-84%25.txt) |

The percentage in each filename is the headline return from the original 4h backtest. Re-run with your own date range, fees, and leverage before relying on it.
