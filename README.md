-----

# Pharos Airdrop Automation Suite 🤖

This Python-based script automates interactions with the Pharos Testnet, helping you to efficiently manage daily tasks for multiple accounts. It supports token swaps, liquidity provision, and daily check-ins to maximize your airdrop potential.

-----

## ✨ Features

  - **Multi-Account Support**: Runs tasks for multiple wallets simultaneously.
  - **Automated Swaps**: Executes token swaps between PHRS, USDC, and USDT.
  - **Liquidity Provision**: Automatically adds liquidity to specified pools.
  - **Daily Check-in & Faucet**: Performs daily sign-ins and claims from the PHRS faucet.
  - **Proxy Integration**: Uses proxies to assign a unique IP for each wallet.
  - **Customizable Configuration**: Easily adjust settings like swap cycles and timeouts.

-----

## 🚀 Getting Started

Follow these steps to get the bot up and running.

### 1\. Prerequisites

  - **Python ≥ 3.10** – [Download Python]([https://www.python.org/downloads/](https://www.python.org/downloads/release/python-3118/))

### 2\. Installation

1.  **Clone the repository:**

    ```sh
    git clone https://github.com/roidlabs/pharos-testnet-bot.git
    cd pharos-testnet-bot
    ```

2.  **Install the required dependencies:**

    ```sh
    pip install -r requirements.txt
    ```

### 3\. Configuration

1.  **`wallet.txt`**: Create this file and add your private keys, one per line.

    ```
    0x...your_private_key_1
    0x...your_private_key_2
    ```

2.  **`proxy.txt`**: Create this file and add your proxies, one per line. The number of proxies must match the number of wallets.

    ```
    http://user:pass@ip:port
    http://ip:port
    socks5://user:pass@ip:port
    socks5://ip:port
    ```

4.  **`config.json`**: Modify this file to adjust the script's behavior.

      - `THREAD_TIMEOUT_MINUTES`: Max time a task can run before timing out.
      - `SWAP_CYCLES`: Number of swap operations to perform.
      - `RETRY_DELAY_MS`: Delay in milliseconds before retrying a failed action.
      - `TRANSACTION_RECEIPT_TIMEOUT_SECONDS`: Max time to wait for a transaction confirmation.

-----

## 💻 How to Run

Execute the main script from your terminal:

```sh
python main.py
```
![main](https://i.ibb.co/ksPqYNR1/image.jpg)

You will see a menu with the following options:

  - **1. Execute Swap & Liquidity Operations**: Runs the trading and liquidity module.
  - **2. Perform Daily Check-in & Faucet Claim**: Runs the daily sign-in and faucet module.
  - **0. Exit Application**: Safely closes the application.

-----

## ⚠️ Disclaimer

This script is provided for educational purposes only.
