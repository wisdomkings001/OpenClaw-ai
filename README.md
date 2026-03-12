# OpenClaw AI — Crypto Intelligence Platform

OpenClaw AI is an all-in-one cryptocurrency trading dashboard that runs entirely in your browser. It combines live Binance market data, AI-powered analysis, paper trading simulation, automated trading bots, and a DCA calculator — no installation required.

---

## Getting Started

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge recommended).
2. The platform loads immediately with live market data from Binance for 50+ tracked coins.
3. To unlock AI-powered features, click **⚙ AI Provider** in the top toolbar and paste your Anthropic API key.
4. To place real trades, click **⬡ Binance Live** and connect your Binance API credentials.

---

## Navigation

The interface is organized into five tabs at the top of the screen:

| Tab | Purpose |
|-----|---------|
| **Market** | Live prices, coin list, and detailed coin view |
| **Trading** | Paper trading simulator with AI analysis |
| **Bot** | Conversational AI assistant for crypto questions |
| **Trades** | Positions, P&L history, live trading, and AutoBot |
| **⬡ DCA** | Dollar Cost Averaging calculator and planner |

---

## Features

### 📈 Market Tab
- **Live Ticker** — A scrolling ticker at the top displays real-time prices and 24h changes for all tracked coins, pulled directly from Binance WebSocket streams.
- **Coin List** — Browse 50+ cryptocurrencies sorted by market activity. Each coin card shows the current price, 24h percentage change, and a color-coded direction indicator.
- **Coin Detail View** — Tap any coin to open a full detail panel showing price, volume, high/low ranges, and a live TradingView chart.

---

### 💹 Trading Tab
- **Paper Trading Simulator** — Start with a virtual $10,000 balance and practice trading without risking real money. Buy and sell coins at live market prices.
- **AI Coin Analysis** — Select any coin and tap **🤖 Analyze** to receive a full AI-generated report including:
  - Support and resistance levels
  - Momentum and trend assessment
  - Recommended entry and exit price zones
  - AI-calculated stop loss and take profit targets
  - Short-term, mid-term, and long-term price forecasts
  - Web-search-enriched insights from analyst opinions and market sentiment
- **Balance Tracking** — Your virtual portfolio balance updates in real time as the market moves.
- **Reset Button** — Use the **Reset** button in the toolbar to restore your paper balance to $10,000 at any time.

---

### 🤖 Bot Tab
- **AI Chat Assistant** — An interactive chat interface powered by your configured AI provider. Ask anything about crypto markets, trading strategies, technical indicators, or specific coins.
- **Quick Questions** — Pre-built buttons let you instantly ask common questions such as:
  - BTC analysis
  - Best momentum coins today
  - RSI explanation
  - Stop loss guidance
  - DeFi and yield farming overview
  - General trading risks
- **Context-Aware** — The bot is aware of live market data and your current paper trading balance, allowing it to give personalized, relevant responses.

---

### 📊 Trades Tab

#### Paper Trading Overview
- **Portfolio Stats** — View your total virtual balance, open position count, realized P&L, and win rate at a glance.
- **Open Positions** — A live list of all your current simulated holdings with entry price and current P&L.
- **30-Day P&L History** — A bar chart showing your daily gains and losses over the past month.
- **Trade History** — A complete log of every simulated trade you have made, including symbol, direction, size, and outcome.

#### ⬡ Binance Live Trading
Connect your real Binance account to place actual orders without leaving the platform:
1. Click **Connect Account** inside the Trades tab (or **⬡ Binance Live** in the toolbar).
2. Enter your Binance API Key and Secret Key. Keys are stored locally in your browser only and are never sent to any external server.
3. Once connected, the live badge turns green and your real USDT and BTC balances are shown.
4. Place **Market** or **Limit** buy/sell orders for any USDT trading pair directly from the order panel.
5. Open orders are displayed and refreshed automatically.

> ⚠ **Security:** Create a dedicated API key for this app. Enable Spot Trading permissions only. Never enable withdrawal permissions.

#### 🤖 AutoBot — Automated Trading
- Toggle the AutoBot on from the **🤖 AutoBot** button in the toolbar.
- Configure trade size, minimum confidence threshold, stop loss %, and take profit %.
- The bot runs every 5 minutes, scans all tracked coins using the AI engine, and places paper trades automatically when a signal meets your confidence threshold.
- All AutoBot activity is logged in real time within the Trades tab.

---

### ⬡ DCA Tab — Dollar Cost Averaging

The DCA tab helps you plan and optimize a recurring investment strategy.

- **DCA Calculator** — Enter your chosen coin, investment amount per period, frequency (daily / weekly / bi-weekly / monthly), and time horizon (1–36 months).
- **DCA Results** — Instantly see projected total invested, estimated coin quantity accumulated, and average cost basis.
- **Buy Schedule** — A table showing the next 8 scheduled purchase dates with estimated prices and cumulative totals.
- **Visual Chart** — A bar chart illustrating how your invested capital and coin holdings grow over time.
- **🤖 AI Strategy Insight** — Request an AI-generated assessment of your DCA plan for the selected coin, including whether it is a strong DCA candidate, what market conditions to monitor, and timing tips.
- **DCA Education** — An expandable explainer covering what DCA is and why it is a popular risk-reduction strategy.

---

### 🧠 AI Float Panel
- A small floating panel appears over the interface whenever a coin is being tracked.
- It displays the AI's current signal (bullish / bearish / neutral) for the active coin along with a live price feed.
- Use **▲ Trade It** to act on the AI's suggestion, **✓ Correct** to confirm the signal was right, or **✗ Wrong** to mark it incorrect.
- The panel tracks how many trades it has learned from, improving signal calibration over time.
- The panel is draggable — click and drag it anywhere on screen.

---

## AI Provider Setup

OpenClaw AI uses the Anthropic API to power its analysis, chat bot, and DCA insights.

1. Click **⚙ AI Provider** in the top toolbar.
2. Paste your Anthropic API key into the input field.
3. Your key is saved in your browser's local storage and is never transmitted to any third-party server.

> You can obtain an API key from [console.anthropic.com](https://console.anthropic.com).

---

## Technical Notes

- **No backend required** — The entire application runs as a single HTML file in the browser.
- **Data source** — Live market prices are streamed from Binance public WebSocket and REST APIs. No Binance account is required for market data.
- **Local storage** — Your paper trading balance, trade history, Binance API keys, and AI provider key are all saved in your browser's local storage.
- **Privacy** — No user data is collected or sent to any server other than Binance (for market data and live orders) and Anthropic (for AI features when you trigger them).
- **Compatibility** — Works in all modern browsers. Best experienced on desktop due to the multi-panel layout.

---

## Disclaimer

OpenClaw AI is a trading tool for educational and informational purposes. AI-generated analysis and forecasts are not financial advice. Paper trading results do not guarantee real trading performance. Live trading involves real financial risk — only trade with funds you can afford to lose.
