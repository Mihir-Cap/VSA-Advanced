# VSA Volume Spread Analysis [Advanced] – Pine Script Indicator

This is a Pine Script-based technical analysis indicator for **TradingView**, designed to visualize Volume Spread Analysis (VSA) concepts on the price chart. The indicator uses volume, candle spread, and close location to identify supply/demand-based price behavior using advanced Wyckoff-based logic.

---

## 📌 Features

This script identifies and labels important VSA patterns on the chart:

- 🔴 **Upthrust** – Wide spread up, closes low, high volume (potential distribution)
- 🟠 **No Demand** – Small spread up bar, low volume, closes in upper third
- 🟢 **Stopping Volume** – Down bar on high volume, closes off lows (potential support)
- 💚 **Test Bar** – Down bar on low volume, closes in top third (bullish test)
- 🌸 **Buying Climax** – Wide spread up on very high volume, closes off highs
- 🔵 **No Supply** – Small down bar on low volume, closes in bottom third
- 🟦 **Effort to Rise** – Wide spread up, high volume, strong close
- 🟥 **Effort to Fall** – Wide spread down, high volume, weak close
- 🔺 **Trap Up Move** – Breaks recent high but closes weakly on high volume
- 🔻 **Trap Down Move** – Breaks recent low but closes strong on high volume

Each pattern is plotted directly on the chart with a distinct shape, color, and label for easy recognition.

---

## ⚙️ Inputs

| Parameter              | Description                                 | Default |
|------------------------|---------------------------------------------|---------|
| Volume SMA Length      | Length of the Simple Moving Average on Volume | 20      |
| High Volume Multiplier | Multiplier to define what is "high" volume  | 1.5     |
| Low Volume Multiplier  | Multiplier to define what is "low" volume   | 0.5     |

---

## 📊 How It Works

This indicator calculates:
- **Volume SMA** – to establish volume thresholds
- **Spread** – candle's high minus low
- **Body size** – absolute difference between open and close
- **CLV (Close Location Value)** – to understand where the candle closes within its range

Then, based on VSA logic and conditions for volume/spread/close location, it plots shapes and alerts when specific patterns are detected.

---

## 🛠️ Usage Instructions

1. Open [TradingView](https://tradingview.com/)
2. Go to the **Pine Script Editor**
3. Paste the contents of `VSA_Advanced_Indicator.pine`
4. Click **Add to Chart**
5. Use the settings panel to adjust volume multipliers and length as needed

---

## 🧠 Strategy Notes

This tool is **not a buy/sell signal generator**, but rather a **contextual analysis tool** to help traders:
- Detect supply/demand imbalances
- Spot distribution/accumulation phases
- Confirm price action with volume

It’s most effective when combined with trend structure, support/resistance zones, and other Wyckoff tools.

---

## 🔔 Alerts

This indicator includes alert conditions for:
- Upthrust
- Stopping Volume
- Test Bar
- Buying Climax
- Trap Up Move
- Trap Down Move

You can create TradingView alerts based on these conditions for real-time monitoring.

---

## 🪪 License

MIT License – Free to use, modify, and distribute with attribution.

---

## 👨‍💻 Author

Created by **Mihir Madkaikar**  
For educational and analytical purposes in the Indian and global markets.

---

## 📬 Feedback & Contributions

If you have suggestions or improvements, feel free to open an [Issue](https://github.com/your-username/VSA-PineScript-Indicator/issues) or a Pull Request. Happy trading! 📈
