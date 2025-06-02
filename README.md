# ⚙️ Rise Testnet Automation Bot ⚡



Welcome to **Rise Testnet Automation Bot** — your ultimate **testnet automation tool** with a slick cyberpunk terminal UI powered by Blessed!  
Automate faucet claims, token swaps, deposits, approvals, and more — all from your terminal like a true crypto boss.

---

## 🚀 Features

- Automated Faucet Claims 🚰  
- Token Swapping with random pairs 🔄  
- Liquidity Providing & Deposits 💸  
- Token Approvals ✅  
- Multi-Wallet Support via `accounts.js`  
- Proxy Support for each wallet via `proxies.txt`  
- Cyberpunk Terminal UI with animations & emojis ✨  
- Real-time Logging with status colors & progress updates  

---

## ⚙️ Requirements

- Node.js 14 or higher  
- Linux, macOS, or Termux (Windows users: use WSL)  

---

## 📦 Installation & Setup

1. Clone the repo  
   ```bash
   git clone https://github.com/cryptodai3/RISE-TESTNET-AUTOMATION.git
   ````
 ```bash
   cd RISE-TESTNET-AUTOMATION
````

---

2. Install dependencies

   ```bash
   npm run setup
   ```
---

3. Add your wallets
   Edit `accounts/accounts.js` and add your wallet addresses and private keys securely:

a. Open the wallets file:
```bash
nano accounts/accounts.js
 ```

b. Add your wallets in this format:
   ```js
   module.exports = [
     { address: "0xYourAddress1", pk: "0xYourPrivateKey1" },
     { address: "0xYourAddress2", pk: "0xYourPrivateKey2" },
     // add more wallets here
   ];
   ```
---

4. Add proxies (optional but recommended)

   Create `accounts/proxies.txt` and add one proxy per line matching each wallet:

```bash   
npm install https-proxy-agent
 ```

a. Create or open the proxy list file:
```bash
nano accounts/proxies.txt
 ```

b. Add your proxy URLs — one per line, in the same order as wallets:
   ```
   http://username:password@proxy1-ip:port
   http://username:password@proxy2-ip:port
   ```

---

## ⚡ Running the Bot

Start the bot with:

```bash
node index.js
```

Navigate the interactive menu to select tasks — the bot will run actions for each wallet using its assigned proxy.

---

## 🧠 Tech Stack

* Node.js
* Ethers.js
* Solidity + solc
* Blessed (Terminal UI)
* dotenv for environment variables
* fs, path, timers for core functionality

---

## 🔐 Security Notice

* NEVER share or commit your private keys publicly.
* Use `.gitignore` to protect `accounts.js` and `.env`.
* Proxies help mask your requests — recommended to use reliable paid proxies.

---

## Author & Credits

**Happy Farming!** 🚀🌾 

*Brought to you by [CryptoDai3](https://t.me/cryptodai3) & [YetiDAO](https://t.me/YetiDAO)*
---

## 🔒 Safety & Support

### ⚠️ Important Disclaimer

- **Testnet Only** - This tool is designed for testnet environments only
- **No Liability** - Use at your own risk. Developers assume no responsibility
- **DYOR** - Always do your own research before using any automation tools
---

### 🛡️ Security Best Practices

- 🔐 Never use Main wallets
- 🚫 Never expose sensitive credentials
- 📜 Always review code before execution
- 💸 Use burner wallets with test tokens only
---

### 💬 Need Help?

- 🐛 **Bug Reports**: [Open a GitHub Issue](https://github.com/cryptodai3/RISE-TESTNET-AUTOMATION/issues)
- 💡 **Channel**: Join [@cryptodai3](https://t.me/cryptodai3)
- 🌐 **Community**: Join [YetiDAO Telegram](https://t.me/YetiDAO)
---

### 🙌 Support Our Work

Love this tool? Help us improve:
- ⭐ **Star the repository**
- 🔗 **Share with your farming community**
- 💎 **Use our referral codes** (where applicable)
- 💡 **Contribute ideas and code**

---

## 📜 License
MIT License - Free for personal and commercial use  
*"With great power comes great responsibility" - Please use wisely*

---
