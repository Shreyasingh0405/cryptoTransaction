# 🚀 Crypto Transactions Fetcher

Welcome to the **Crypto Transactions Fetcher**! This project is a Node.js-based server-side application that allows you to fetch, store, and manage cryptocurrency transactions effortlessly. Whether you're exploring your crypto transactions or tracking the latest Ethereum price, this app has got you covered! 🌟

## 🌟 Features

1. **🔍 Fetch Crypto Transactions**: Easily fetch the "Normal" transactions of a user from the Ethereum blockchain using the [Etherscan API](https://docs.etherscan.io/api-endpoints/accounts). Just input the user's address, and you're good to go!  
2. **💾 Store Transactions in MongoDB**: All fetched transactions are stored in a MongoDB database for quick and easy access.  
3. **⏰ Get Real-time Ethereum Price**: Automatically fetches the current price of Ethereum every 10 minutes using the [CoinGecko API](https://api.coingecko.com/api/v3/simple/price?ids=ethereum&vs_currencies=inr) and stores it in the database.  
4. **📊 Calculate Current Balance and Price**: Input a user's address to get their current balance, calculated based on their transaction history, and the latest Ethereum price in INR.

## 📬 How to Use

### 1. Fetch Crypto Transactions

- **Endpoint**: `GET /api/transactions/:address`  
- **Description**: Provide a user's Ethereum address to fetch and store their transactions in the database.

### 2. Fetch Ethereum Price Every 10 Minutes

- This happens automatically in the background using a scheduled job. The price is stored in the database and updated every 10 minutes.

### 3. Get User Balance and Current Ethereum Price

- **Endpoint**: `GET /api/user-balance/:address`  
- **Description**: Provide a user's Ethereum address to get their current balance (calculated from their transactions) and the latest Ethereum price.

---
