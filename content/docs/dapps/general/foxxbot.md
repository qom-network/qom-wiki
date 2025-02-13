---
title: FoxxBot
type: docs
---
## Introduction to FoxxBot

FoxxBot is an automated trading bot built for the QL1 blockchain, executing trades exclusively on QSwap. Designed for high-frequency trading, it focuses on maximizing profitability while maintaining a deflationary mechanism through a structured buyback and burn system.

FoxxBot operates on the **Wqom/QUSDT trading pair**, targeting 4% profit per trade. It continuously monitors market trends, adjusting its strategy based on Exponential Moving Averages (EMA) and other trading parameters.

Managed and operated exclusively by **FoxxOne**, FoxxBot supports the deflationary supply of $Wqom while ensuring the long-term sustainability of the FoxxOne validator, RPC node, and dApp node infrastructure.

---

## Profit Distribution & Burn Mechanism

FoxxBot employs a structured profit distribution model to ensure sustainable trading operations while actively contributing to the deflationary model of $Wqom.

### Profit Allocation

- **Capital Wallet (75%)** – Used to reinvest into trading, maintaining liquidity and increasing trade volume.
- **Burn Wallet (25%)** – Profits allocated to this wallet are used for buyback and burn of $Wqom, reducing the circulating supply over time.

### Planned Increase in Burn Allocation

To further strengthen the deflationary pressure on $Wqom, FoxxBot’s profit allocation to the Burn Wallet will gradually increase over time. The distribution will shift from **75% capital / 25% burn** to an equal **50/50 split**, ensuring a greater percentage of trading profits are allocated toward buyback and burn.

Additionally, during high-liquidity periods or special burn events, FoxxBot may adjust the allocation to **25% capital / 75% burn**, significantly accelerating the deflationary process. These strategic adjustments will be made based on market conditions and infrastructure sustainability needs.

### How the Burn Wallet Works

🔥 **Automated Burn at 100 QUSDT**  
When the Burn Wallet accumulates 100 QUSDT, it automatically executes a buyback and burn, purchasing $Wqom from QSwap and permanently removing it from circulation.

🔥 **Manual Burn via /burn Command**  
Additional manual burns can be executed as necessary to further reduce $Wqom supply.

---

## FoxxBot Commands & Features

FoxxBot includes commands for monitoring and fine-tuning its trading parameters.

### 🤖 Trading Commands

- `/buy X` – Manually buy Wqom with QUSDT (Min: $1, Max: $20)
- `/sell X` – Manually sell Wqom for QUSDT
- `/balance` – Show wallet balances
- `/profit` – Display profit & loss (QUSDT $ value) and trade statistics
- `/profit% X` – Set sell profit target percentage (Current: 4.00%)
- `/dynamic` – Toggle dynamic profit adjustment (Current: ON)
- `/settings` – Display current bot settings and number of open trades

### 🔥 Burn & Reset Commands

- `/burn` – Swap Burn Wallet QUSDT → Wqom and burn the Wqom
- `/reset` – Reset EMA, profit settings, trade & price history, and persistent P&L

### 📊 Bot Configuration Commands

- `/ema ####` – Set EMA window (1 to 2000) (Current: 80)
- `/buythreshold X` – Set buy threshold multiplier (Range: 1.02 to 1.04, Current: 1.03)
- `/dca [on|off]` – Toggle DCA (Dollar-Cost Averaging) feature on or off

---

## Current Bot Settings

The following settings determine how FoxxBot operates and executes trades:

| **Setting**               | **Value**      | **Description**                                           |
|---------------------------|----------------|-----------------------------------------------------------|
| **EMA Period**            | 80             | Determines the Exponential Moving Average window for trend tracking |
| **Buy Threshold Multiplier** | 1.03         | The price must exceed EMA × multiplier for a buy to trigger |
| **Sell Profit Target**    | 4.00%          | The bot will sell when profit reaches the set percentage   |
| **Min Buy Amount**        | $1.00          | Minimum trade size per transaction                         |
| **Max Buy Amount**        | $20.00         | Maximum trade size per transaction                         |
| **Max Open Trades**       | 40             | The bot can open up to 40 simultaneous trades              |
| **Trade Interval**        | 45 seconds     | Minimum time between trade executions                      |
| **Slippage Tolerance**    | 3%             | Acceptable slippage percentage for trade execution         |
| **Dynamic Profit Adjustment** | ON          | The bot dynamically adjusts trade strategies based on market conditions |
| **Open Trades**           | 30             | Number of currently open trades                            |
| **DCA Enabled**           | ON             | Dollar-Cost Averaging is enabled for strategic trading     |

---

## Dollar-Cost Averaging (DCA)

### How DCA Works

FoxxBot’s **DCA functionality** enhances trading profitability by strategically averaging down the entry price of open trades. When conditions are met, the bot executes additional purchases on existing trades, improving the chances of hitting the sell target.

### Key Features of DCA

- **Trigger Conditions:** DCA is initiated when the price moves a set percentage away from the original buy price.
- **Controlled Buy Amounts:** The bot allocates a fraction of the original trade size for DCA buys, ensuring capital is preserved.
- **Maximum DCA Attempts:** A limit is set on the number of DCA attempts per trade to manage risk.

---

## How FoxxBot Supports the QL1 Ecosystem

FoxxBot is a critical component of the QL1 ecosystem, designed to:

✔️ Provide consistent trading volume on QSwap  
✔️ Create continuous buying pressure through automated buybacks  
✔️ Reduce the supply of $Wqom through its structured burn mechanism  
✔️ Ensure the ongoing operation of key blockchain infrastructure, including the FoxxOne validator, RPC node, and dApp node  

By running efficiently and autonomously, FoxxBot helps maintain a sustainable ecosystem while contributing to the long-term value of $Wqom.

---

## How to Stay Updated

All burn events, trading statistics, and future updates will be shared through the official FoxxOne channels:

🌐 **Official Website:** [FoxxOne.one](https://foxxone.one)  
📢 **Telegram Announcements**

---

## FoxxBot Development Team

**Powered by FoxxOne.one** – Driving innovation in QL1 blockchain analytics and automation.
