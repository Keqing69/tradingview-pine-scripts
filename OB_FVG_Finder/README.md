# SMC Scanner [FVG + OB]

A clean, automated tool to find **Fair Value Gaps** and **Order Blocks** on any timeframe.
It focuses on keeping your chart organized by automatically removing old or invalid zones.

![Preview](/Users/keqing/Documents/TradingViewScripts/OB_FVG_Finder/preview.png)

*(Make sure to add your screenshot named `preview.png` to the images folder)*

## ⚡ What it does

* **Order Blocks (OB):** Highlights strong reversal zones where institutional money likely entered the market.
* **Fair Value Gaps (FVG):** Marks imbalances in price action that often act as magnets for price to return to.
* **Auto-Cleanup:** Unlike other indicators, this script deletes zones that are too old or have been "mitigated" (filled) to prevent chart clutter.

## ⚙️ How it works

1.  **Momentum Detection:** It compares the current candle size to the average of the last 20 candles. If a move is strong enough, it marks an **Order Block**.
2.  **Gap Detection:** It looks for 3-candle patterns where price skipped a level, creating a **Fair Value Gap**.
3.  **Smart Management:**
    * **Fixed Length:** Boxes only extend a few bars into the future so you focus on *current* price action.
    * **Mitigation:** If price fills an FVG, the box is removed or grayed out immediately.

## 🔧 Key Settings
* **Extension:** How far the boxes draw into the future.
* **Momentum Multiplier:** Increase this to find only the *strongest* Order Blocks.
* **Hide Mitigated:** Turn this on to instantly delete FVGs once price touches them.

---
*Use at your own risk. For educational purposes only.*