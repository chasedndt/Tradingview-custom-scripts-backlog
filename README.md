
1. # Combo Confirmed FVG
An enhanced Fair Value Gap (FVG) indicator that only triggers alerts when a gap is tapped *and* confirmed by trend alignment using EMA 21/55.

---

## 🔍 What It Does

- Detects 3-bar Fair Value Gaps (Bullish and Bearish)
- Filters invalid gaps using a customizable minimum gap % size
- Monitors FVGs until they are tapped
- Confirms tap only when EMA 21 > EMA 55 (for bullish) or EMA 21 < EMA 55 (for bearish)
- Triggers alert when both gap fill AND EMA alignment are met
- Optionally hides boxes after fill

---

## 🧠 Why It Matters

This script eliminates weak or out-of-trend FVG setups by combining structural imbalance with momentum confirmation, giving higher-probability entries.

---

## ⚙️ Inputs

- `FVG life (bars)` – how long the gap box should stay on chart
- `Min gap %` – minimum required gap size as % of price
- `Box transparency` – visual opacity of the FVG
- `Fill % to count as tap` – how much of the box must be filled to trigger alert
- `Hide box once filled` – whether to remove the FVG after tap
- `Enable alerts` – whether to activate the Discord/webhook alert system

---

## ✅ Alert Condition

| Title | Message |
|-------|---------|
| ⚡ Combo FVG Confirmed | `{ "content": "⚡ {{ticker}} ({{interval}}) triggered a COMBO FVG ENTRY." }` |

You can use this to set up TradingView alerts with Discord webhooks.

---

## 🔌 Use in Live Trading

Works across multiple timeframes (suggested: 1H, 15m, 4H). Add it to your preferred charts, set alerts per pair, and receive precision entry signals in real time.

---

## 📎 Example Use Case

Add to BTCUSDT 1H chart → Create alert → Paste Discord webhook → Done.
Repeat across other pairs like ETH, SUI, SOL, XRP.

---

## 🚀 Author

Built by the Blockchain Boys team. For advanced crypto traders using smart money concepts and algo-assisted execution.
