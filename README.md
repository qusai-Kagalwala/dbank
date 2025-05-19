# DBank - Decentralized Banking Application

A decentralized banking application built on the Internet Computer blockchain that allows users to perform basic banking operations in a trustless, decentralized environment.

## 🚀 Features

- **Deposit & Withdrawal**: Secure deposit and withdrawal of digital assets
- **Balance Tracking**: Real-time balance monitoring
- **Interest Calculation**: Automated interest accrual on deposits
- **Transaction History**: Complete record of all banking activities
- **Decentralized**: No central authority or single point of failure
- **Secure**: Built on Internet Computer's secure blockchain infrastructure

## 🛠️ Technology Stack

- **Backend**: Motoko (Internet Computer)
- **Frontend**: React.js
- **Blockchain**: Internet Computer Protocol (ICP)
- **Development Framework**: DFX (DFINITY SDK)
- **Package Manager**: NPM

## 📋 Prerequisites

Before running this project, make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [DFINITY SDK (DFX)](https://sdk.dfinity.org/docs/download.html)
- Git

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/qusai-Kagalwala/dbank.git
   cd dbank
   ```

2. **Install NPM dependencies**
   ```bash
   npm install
   ```

3. **Install DFX (if not already installed)**
   ```bash
   sh -ci "$(curl -fsSL https://sdk.dfinity.org/install.sh)"
   ```

## 🚀 Running the Application

### 1. Start the Local Internet Computer Replica
```bash
dfx start --clean
```

### 2. Deploy the Canisters
In a new terminal window:
```bash
dfx deploy
```

### 3. Start the Frontend Development Server
```bash
npm start
```

The application will be available at `http://localhost:3000`

## 📁 Project Structure

```
dbank/
├── src/
│   ├── dbank/
│   │   └── main.mo          # Main Motoko backend logic
│   └── dbank_assets/
│       ├── src/
│       │   ├── index.js     # Frontend JavaScript
│       │   └── index.html   # HTML template
│       └── assets/          # Static assets
├── .dfx/                    # DFX configuration
├── dfx.json                 # Project configuration
├── package.json             # NPM dependencies
└── README.md               # This file
```

## 🔑 Core Functionality

### Banking Operations
- **Deposit**: Add funds to your account
- **Withdraw**: Remove funds from your account (with balance validation)
- **Check Balance**: View current account balance
- **Interest**: Automatic compound interest calculation

### Smart Contract Features
- Immutable transaction records
- Overflow protection for large numbers
- Time-based interest calculations
- Secure access controls

## 🧪 Testing

Run the test suite:
```bash
dfx test
```

## 📝 Usage Example

```javascript
// Check current balance
const balance = await dbank.checkBalance();

// Make a deposit
await dbank.topUp(100);

// Withdraw funds
await dbank.withdraw(50);

// Get compound interest
await dbank.compound();
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- [Internet Computer Documentation](https://internetcomputer.org/docs/)
- [DFX SDK Documentation](https://sdk.dfinity.org/)
- [Motoko Programming Language](https://internetcomputer.org/docs/current/motoko/intro/)

## 👤 Author

**Qusai Kagalwala**
- GitHub: [@qusai-Kagalwala](https://github.com/qusai-Kagalwala)

## 🐛 Issues

Found a bug? Please report it [here](https://github.com/qusai-Kagalwala/dbank/issues).

## 📞 Support

If you have any questions or need help, please open an issue or contact the maintainer.

---

⭐ If you found this project helpful, please give it a star on GitHub!
