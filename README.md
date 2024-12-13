# Datapig XYZ Bot

This repository contains a bot designed to interact with the [Datapig API](https://app.datapig.xyz). The bot can generate random preferences, sign messages, generate analysis, and mint files to the blockchain. It runs every 24 hours to process wallets automatically.

## Features

- **Automatic Wallet Processing**: It processes each wallet's data, generates preferences, signs messages, and submits them.
- **Retry Mechanism**: The bot retries minting files in case of failure (up to 3 retries).
- **Daily Limit Handling**: Automatically detects and handles the "Daily Limit Reached" response from the Datapig API and moves on to the next wallet.
- **Scheduled Execution**: The bot runs every 24 hours, automatically processing the wallets at the set interval.

---

## Requirements

Before you begin, ensure that you have met the following requirements:

- **Node.js**: Version 16 or higher.
- **npm**: Package manager to install dependencies.
- **Private keys** for the wallets you want to interact with.
- **Reference Codes** (optional but recommended for additional rewards) for your wallets.

---

## Installation

Follow these steps to set up the project on your local machine:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ganjsmoke/datapig-xyz.git
   cd datapig-xyz
   ```
2. **Install Dependencies**:
  ```bash
  npm install
  ```

3. **Setup private_keys.txt**
   
Create a file named private_keys.txt in the root directory of the project. REF_CODE is the account that referes you
```bash
<PRIVATE_KEY_1>,<REF_CODE_1>
<PRIVATE_KEY_2>,<REF_CODE_2>
```

---

## Running Bot

Once you've completed the setup, you can run the bot with the following command:

```bash
node index.js
```

This will process each wallet in the private_keys.txt file, generate random preferences, sign messages, submit them to the Datapig API, and mint files to the blockchain. The bot will repeat this process every 24 hours.

---

## Support

If you encounter any issues or need further assistance:

- **Bot Support: t.me/airdropwithmeh
