# Solana Prediction Market Smart Contract

A decentralized prediction market platform built on Solana blockchain, inspired by Polymarket. This project enables users to create markets, trade positions, and resolve outcomes based on real-world events.

## Features

- **Market Creation**: Create prediction markets for any event
- **Liquidity Provision**: Add and withdraw liquidity to markets
- **Trading**: Trade positions using Yes/No tokens
- **Market Resolution**: Automatic resolution based on final outcomes
- **Fee Structure**: Platform and LP fees for sustainable operations

## Architecture

The project is built using:
- Solana Web3.js
- Anchor Framework
- SPL Token Program
- Associated Token Program

## Getting Started

### Prerequisites

- Node.js
- Yarn
- Solana CLI
- Anchor Framework

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/solana-prediction-market.git
cd solana-prediction-market
```

2. Install dependencies:
```bash
yarn install
```

3. Build the program:
```bash
anchor build
```

### Configuration

Configure your project settings:
```bash
yarn script config -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

### Usage Examples

1. Create a new market:
```bash
yarn script market -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

2. Add liquidity to a market:
```bash
yarn script addlp -y <yes-token-address> -n <no-token-address> -a <amount> -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

3. Trade positions:
```bash
yarn script swap -y <yes-token-address> -n <no-token-address> -a <amount> -s <style> -t <token-type> -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

4. Withdraw liquidity:
```bash
yarn script withdraw -y <yes-token-address> -n <no-token-address> -a <amount> -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

5. Resolve market:
```bash
yarn script resolution -y <yes-token-address> -n <no-token-address> -e devnet -k <your-keypair-path> -r <your-rpc-url>
```

## Example Transactions

### Configuration
[View Transaction](https://solscan.io/tx/3PsfbvzAPyhwNPQm2aCTf3XUaJwwrZTCoVVw41uJMzs3DXvx948JUrtW2KQRH1UkoTNFxMSbpN32KF5aFQuZ7mCc?cluster=custom&customUrl=https://api.devnet.solana.com)

### Market Creation
[View Transaction](https://solscan.io/tx/4xnzHarhppyWKJccQh27TUCTyeR2da8JGSXWsKAYw5YvVywKKWJzSz9JxRzNwhuj7fjmrCAhtM2drWc29a8J3i2C?cluster=custom&customUrl=https://api.devnet.solana.com)

### Add Liquidity
[View Transaction](https://solscan.io/tx/3kfdmxfq1U6JKwo7p5aAHQ2QeaF6pxp41ycN2wDTBToujEWQMewSfNpwCSBTLuxFsy1MAUojqfkWkAqAMo63b94k?cluster=custom&customUrl=https://api.devnet.solana.com)

### Withdraw Liquidity
[View Transaction](https://solscan.io/tx/5QDonNfWURYyGrQQwTQWjccsnmRuWSNDb66WuuXo12cWhwXo2SwbvSrRpimXPkAbsSmMzD8iYaoEdf5CgMFdtEk3?cluster=custom&customUrl=https://api.devnet.solana.com)

### Swap
[View Transaction](https://solscan.io/tx/5s9xy2no9YANBCsp8Zr5fBq6whHK65t7eBU3AxLp6xFNcagvvzhpknWrJHrk8BYLfnf4jF6kzeW4QyuZi4UUKQKX?cluster=custom&customUrl=https://api.devnet.solana.com)

### Resolution
[View Transaction](https://solscan.io/tx/TryUfcHXKTVWTY3vM1bUCckbtBCxnHBrbB92LFCpRf67J5po2HsqvPT5wWNYSQJVWBcvcvWbS42KfcX6vufdUup?cluster=custom&customUrl=https://api.devnet.solana.com)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
