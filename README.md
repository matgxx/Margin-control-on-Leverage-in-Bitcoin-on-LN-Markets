LN Markets Telegram Trading Bot

This is an automated Python trading bot designed for the LN Markets Futures platform. It implements a DCA (Dollar-Cost Averaging) strategy on price dips and features full Telegram integration for real-time monitoring, critical alerts, and remote configuration management.

Key Features
DCA Strategy: Opens new Long positions in the futures market when the price drops by a predefined amount from its recent peak.

Risk Management (Guardian Angel): Actively monitors open positions and automatically adds safety margin if the liquidation price gets too close.

Automatic Take Profit: Sets a profit target for each position upon opening.

Telegram Integration:

Alerts: Receive instant notifications for buys, position closures, and liquidation alerts (margin additions).

Reports: Sends periodic status reports including balance, current price, and open positions.

Remote Control: Manage the bot (Pause/Resume, Status) using inline buttons in the chat.

Configuration: Change strategy parameters (like BUY_DROP_AMOUNT, MAX_POSITIONS, etc.) directly via Telegram.

Quick Setup:
Prerequisites
Python 3.x
An active LN Markets account.
A Telegram bot (create one using BotFather).


Install dependencies
pip install ln-markets requests urllib3


API_KEY = "YOUR_API_KEY"
API_SECRET = "YOUR_API_SECRET"
PASSPHRASE = "YOUR_PASSPHRASE"
NETWORK = "mainnet" or "testnet"

Telegram Credentials 
TELEGRAM_BOT_TOKEN = "YOUR_BOT_TOKEN"
DEFAULT_TELEGRAM_CHAT_ID = 123456789 Your chat or group ID

