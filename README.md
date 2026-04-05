
# BSC/EVM Generalized Frontrunning Token Sniping MEV Bot for Pancakeswap

A generalized token-sniping bot for tokens when they launch on EVM-compatible networks (BSC, ETH, AVAX, MATIC, FTM, CRO, ONE, MilkADA, Moonforce, etc). Intended for testing, research, and educational purposes. Use at your own risk.

This project is provided for research and educational purposes only. Use responsibly and in accordance with applicable laws and platform terms.

## Features

- ⚡ Lightning-fast token sniping
- 🥞 PancakeSwap V2 support
- 💸 Auto-claim funds
- 🔒 Secure private key management (never leaves your machine)
- 💰 Designed to maximize profit during new token launches and liquidity events
- 🛡️ Anti-rugpull, anti-honeypot checks (optional)
- 📈 Real-time monitorings
- 💫 Multi-chain EVM support
- Mempool transaction decoding (via `abi-decoder`)
- Web3-based interaction with nodes (`web3`)
- Configurable runtime parameters (see `env.js` and `constants.js`)

## Requirements


- Node.js and npm (LTS recommended, Linux recommended)
- Windows users: Visual Studio C++ Build Tools (only if native modules are required)

## Getting Started

1. Install dependencies:
   
   ```bash
   npm install
   ```

2. Configure environment:
   - Update `env.js` with your RPC endpoints and credentials (e.g., private key).
   - Adjust `constants.js` for chain IDs, contract addresses, gas settings, and other operational parameters.

3. Run the bot:

   ```bash
   node token-sniper.js
   ```

## Configuration

- `env.js`: Sensitive runtime values such as RPC URLs and private keys. Keep this file secure and never commit secrets.
- `constants.js`: Network and application constants (e.g., router addresses, WETH/WBNB addresses, gas multipliers).

Feel free to reach out for implementation assistance or integration support.

## Security Notes

- Never commit private keys or credentials.
- Prefer environment variables or a secrets manager in production.
- Use dedicated wallets and risk controls when operating on mainnet.

## Legal Disclaimer

This software is provided “as is,” without warranty of any kind. You are solely responsible for compliance with laws, exchange/DEX terms, and all risks (including financial loss) arising from use of this software.

This tool is for educational purposes only. Use at your own risk. The author is not responsible for any financial losses or legal issues.

## How to convert seed phrase to a private key?
A lot of cryptowallets don't provide you the private key, but just the seed phrase (12 words). If you do not have your private key, it is easy to find:
This video [Here](https://youtu.be/eAXdLEZFbiw) will tell you the instructions. Website I used is [this one](https://iancoleman.io/bip39/) but you can find others on Youtube or just check github.


## FAQ

**Q: Is this safe?**
A: The bot never uploads your private key. All transactions are signed locally.

**Q: Is this legal?**
A: This is for educational and research purposes only. Use at your own risk.

**Q: How much can I expect to make in a day?**
A: I managed to turn 0.1 BNB into 2 BNB in 1 day, however your results maybe different. You may make more than when I first tested this tool.

## Binaries

Precompiled binaries are not provided in this repository. Build and run from source as described above.
