# The Box Theory

These indicators identify breakouts or bounces and then seek a suitable candle for entry. No strategy is 100% reliable, and all traders experience losses at times. The most important thing is to manage risk properly and make sure profits outweigh losses.

These strategies were created and are maintained by [Timo Anttila](https://github.com/timoanttila). If you have suggestions or ideas, feel free to reach out. The scripts were built for [TradingView](https://www.tradingview.com/), a widely used platform for technical analysis and trading.

Day trading is risky, and most traders lose money. Only trade money you can afford to lose, and test your strategy in a simulator first. This content is for education and information only - not investment advice. Always do your own research and backtest before making any decisions.

---

## Opening Range with Breakouts

[Opening Range with Breakouts](./OpenRange.pine) is based on the long-standing **Opening Range Breakout (ORB)** strategy, a method popularized by legendary traders like Toby Crabel and Mark Fisher. It's a simple yet powerful tool for identifying and trading breakouts from the opening ranges of the London and New York trading sessions.

The script provides a clear visual representation of the opening range on your chart, then signals potential entry points once a breakout with a pullback occurs.

### How It Works

The core of the strategy is to first establish the opening range, which is the high and low price within the first 15 minutes of a new trading session. Once this range is set, the indicator monitors for a **breakout** - when the price moves and closes beyond either the OR high or OR low.

While some ORB strategies involve a direct entry on the breakout, this indicator looks for a **pullback**, or a brief counter-move back towards the range before the trend resumes. By waiting for this pullback, the indicator helps filter out false breakouts and provides more reliable entry signals.

A **buy or sell signal** is then plotted on the chart when the price moves past the high or low of the pullback candle, confirming the continuation of the breakout.

### Features and Usage

The indicator provides a structured, consistent basis for judging daily price action and determining whether a day is likely to be a "range day" or a "trend day."

#### Customizable Sessions

 You can easily adjust the start and end times for both the London and New York sessions to fit your trading preferences.

#### Clear Visuals

The OR is displayed as a box on your chart, making it easy to see the established range.

#### Entry Signals

The indicator plots buy and sell signals directly on the chart, helping you quickly identify potential trade opportunities.

### Alerts

The script includes a variety of alert conditions that you can configure to notify you of potential trading opportunities, including any entry, a London entry, a New York entry, or specific bullish and bearish entries.

* **Any Entry**: Triggers on any bullish or bearish entry from either the London or New York sessions.
* **London Entry**: Triggers on any entry specifically from the London session.
* **New York Entry**: Triggers on any entry specifically from the New York session.
* **Any Bullish Entry**: Triggers on any bullish entry from either session.
* **Any Bearish Entry**: Triggers on any bearish entry from either session.

---

## Previous Day's Candle Breakouts and Bounces

[Previous Day's Candle Breakouts and Bounces](./PDB.pine) is a technical analysis tool that plots the **previous day's high, low, open, and midpoint** on the current chart. These levels are often watched by traders as they can act as significant **support and resistance**. The script's primary function is to identify and signal two distinct types of price action at these critical levels: **bounces** and **breakouts**.

### How It Works

The indicator's logic is based on tracking price interaction with these key reference points from the previous day.

#### Bounces / Reversals

The script detects when price approaches the previous day's high or low but is rejected. It uses a customizable buffer zone to account for slight penetrations before the reversal. A signal is generated when price moves back in the opposite direction after testing the level, indicating a potential reversal.

#### Breakouts  / Continuations

The indicator also identifies when price breaks decisively above the previous day's high or below the previous day's low. To increase the reliability of these signals, it incorporates a **pullback** filter. A signal is only triggered after a confirmed breakout is followed by a brief retracement, which is then overcome by price continuing in the original breakout direction. This helps to reduce false signals and confirm the strength of the move.

---

### Signals and Alerts

The script provides clear visual cues on the chart to make these events easy to spot.

* A **circle** is plotted to indicate a **bounce** signal.
* A **triangle** is plotted to indicate a **breakout** signal.

For convenience, you can set up a variety of **alerts** to notify you of these events in real time. This includes alerts for a general "Box Break or Bounce," as well as separate alerts specifically for "Box Break" or "Box Bounce" events.