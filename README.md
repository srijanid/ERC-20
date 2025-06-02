# Ethereum Token Implementations

This repository contains basic implementations of Ethereum token standards:

- [ERC-20](https://github.com/srijanid/ERC-20)
- [ERC-721 (NFT)](https://github.com/srijanid/ERC721-Token)

These smart contracts are written in **Solidity** and deployed/tested using **Remix IDE**, following the official [Ethereum Improvement Proposals (EIPs)](https://eips.ethereum.org/).

---

## 🔁 ERC-20 Token

### Overview
The ERC-20 standard defines a fungible token — each token is identical and interchangeable. This implementation provides basic token functionality including transfer, approval, and allowance handling.

### Features
- `totalSupply`: Returns total circulating tokens.
- `balanceOf`: Gets the balance of an address.
- `transfer`: Sends tokens to another address.
- `approve`: Authorizes another address to spend on behalf.
- `transferFrom`: Executes transfers from authorized accounts.
- `allowance`: Shows how many tokens an address can spend on another's behalf.

### Sample Functions
```solidity
function transfer(address recipient, uint256 amount) public returns (bool)
function approve(address spender, uint256 amount) public returns (bool)
function transferFrom(address sender, address recipient, uint256 amount) public returns (bool)

🚀 FeaturesDeployment & Testing (via Remix)
Open Remix IDE.
Create a new file and paste the contents of MyERC20Token.sol.
Compile the contract using the Solidity compiler.
Deploy the contract using "Deploy & Run Transactions".
Interact with functions such as transfer, approve, transferFrom, etc.

📁 File Structure
bash
Copy
Edit
ERC-20/
└── MyERC20Token.sol   # Main ERC-20 contract

🛠️ Requirements
Solidity ^0.8.0
Remix IDE / Truffle / Hardhat (for testing)
MetaMask or a similar Ethereum wallet

📜 License
MIT License

🙋 Author
Srijan ID
Ethereum Smart Contract Developer | Blockchain Enthusiast

📚 References
EIP-20 (ERC-20)
Solidity Documentation
OpenZeppelin Contracts
