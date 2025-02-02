---
title: Fox Contract Checker
type: docs
---

# 🦊 Fox Contract Checker – Web Version  

**Fox Contract Checker** is a comprehensive on-chain contract analysis tool for the **QL1 blockchain**. Available on the web at **[foxxone.one](https://foxxone.one)**, it enables users to verify token contracts, identify potential risks, and make informed decisions before engaging with any token.

---

## 📌 Features  

### 🔍 **Smart Contract Analysis**  
- Analyze token contracts and identify potential vulnerabilities.  
- Checks for **ownership status** and flags **suspicious functions**.

### 🛡️ **Security Flags**  
- Rates contracts on a **Fox Rating Scale** from 1 to 5:  
  - **1 Fox:** High Risk  
  - **5 Foxes:** Safest  

### ⚠️ **Suspicious Functions Detected**  
The **Fox Contract Checker** reviews contracts for the following prominent vulnerabilities and more:  
- **Minting Functions**: Developer can create unlimited tokens.  
  - Example: `mint(address,uint256)`  
- **Blacklist Functions**: Developer can block wallets from interacting.  
  - Example: `setBlacklist(address,bool)`  
- **Forced Transfers**: Potential for transferring user tokens without consent.  
  - Example: `transferFrom(address,address,uint256)`  
- **Ownership Control**: Allows transfer of contract ownership.  
  - Example: `transferOwnership(address)`  
- **Withdrawal Functions**: Risk of draining user or liquidity pool funds.  
  - Example: `withdraw()`  
- **Self-Destruct Mechanisms**: Contract can destroy itself after malicious activity.  
  - Example: `selfdestruct(address)`  
- **Unrestricted Approvals**: Allows excessive token spending permissions.  
  - Example: `approve(address,uint256)`  

### 📊 **Token Metrics & Insights**  
- Fetches real-time token details such as:  
  - **Name**, **Symbol**, **Decimals**, and **Total Supply**  
  - Liquidity data and trading pairs on **QSwap**  

### ⚡ **Lightning-Fast Checks**  
- Powered by the **FoxxOne RPC Node** for instant blockchain data retrieval.  

### 🖥️ **Simple and Intuitive UI**  
- Input a contract address and receive a clear **risk report** with ratings.  
- Dark theme aesthetics designed for seamless use across devices.  

---

## 🛠️ How It Works  

### 1️⃣ **Analyze a Token Contract**  
1. Visit **[foxxone.one](https://foxxone.one)**.  
2. Enter the contract address in the **Fox Contract Checker** tool.  
3. Click **"Check"** to generate a report.

✅ You’ll receive:  
- Token details such as name, symbol, and supply.  
- A **security risk report** listing suspicious functions and a **Fox Rating**.

### 2️⃣ **Understand the Fox Rating Scale**  

| 🦊 Rating | Risk Level          | Description                          |
|-----------|---------------------|--------------------------------------|
| **1 Fox** | 🔴 High Risk        | Multiple vulnerabilities detected    |
| **2 Foxes** | 🟡 Medium Risk     | Moderate concerns                   |
| **3 Foxes** | 🟠 Average Risk     | Some risks identified               |
| **4 Foxes** | 🟢 Low Risk         | Secure with minor concerns           |
| **5 Foxes** | 🟢 Safest           | No risks detected                   |

---

## 📷 Screenshot  

### Contract Check Tool  

![Fox Contract Checker](https://i.imgur.com/7qzcnZc.png)  

---

## 🔗 Useful Links  

- 🖥️ **Fox Contract Checker (Web):** [foxxone.one](https://foxxone.one)  
- 🌐 **FoxxOne RPC Node:** [json-rpc.foxxone.one](https://json-rpc.foxxone.one)  
- 🔄 **QSwap:** [QSwap Explorer](https://qswap.foxxone.one)  

---
