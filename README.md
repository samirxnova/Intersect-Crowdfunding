# Decentralized Kickstarter dApp

## Introduction

This repository contains the code for a decentralized crowdfunding platform built on the **Avalanche's Intersect Testnet**. Our dApp allows users to create, fund, and manage crowdfunding projects in a trustless and transparent way. We use **Solidity** to manage the smart contracts and **ReactJS** for the frontend. The platform operates on **Avalanche's Intersect Testnet** and uses **Pearl (PEARL)**, the native test token, for all transactions.

## Features

- **Create a Project:** Users can initiate a project by defining a funding goal and deadline.
- **Fund a Project:** Backers can support projects by contributing PEARL tokens.
- **Withdraw Funds:** Project creators can withdraw funds if their project reaches the funding goal before the deadline.
- **Get Refund:** If a project fails to reach its goal, backers can withdraw their contributions.

## Technologies Used

### Blockchain
- **Avalanche Intersect Testnet:** The platform is built on Avalanche’s testnet to leverage low transaction fees and high throughput.
- **Solidity:** Smart contracts written in Solidity manage the project lifecycle, funding, and withdrawals.
  
### Frontend
- **ReactJS:** The frontend is built using ReactJS for a responsive user experience.
  
### Libraries & Tools
- **Web3.js/Ethers.js:** Interacts with smart contracts on Avalanche.
- **MetaMask:** Used for handling authentication and transactions.

## Getting Started

### Prerequisites
- **Node.js** and **npm** installed.
- **MetaMask** browser extension.
- Obtain **PEARL test tokens** from the Avalanche testnet faucet:  
  [Avalanche Intersect Testnet Faucet](https://core.app/en/tools/testnet-faucet/?subnet=intersect&token=intersect)

### Steps to Run the dApp

1. **Clone the Repository**
   ```bash
   git clone https://github.com/samirxnova/Intersect-Crowdfunding.git
   cd Intersect-Crowdfunding
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```
   
3. **Deploy the Smart Contract**
   Use Remix or Truffle to deploy the smart contracts on the Avalanche Intersect Testnet.

4. **Start the Frontend**
   After the contract is deployed, run the frontend:
   ```bash
   npm start
   ```

5. **Test and Interact with the dApp**
   Connect MetaMask to the **Avalanche Intersect Testnet** and interact with the dApp:
   - Create crowdfunding projects.
   - Fund projects using PEARL tokens.
   - Withdraw or request refunds as applicable.

### Setting Up Intersect Testnet in MetaMask

To connect your MetaMask wallet to the Intersect Testnet:

1. Open MetaMask and click on the network dropdown.
2. Select **Add Network** and fill in the following details:

   - **Testnet Name:** Intersect Testnet
   - **EVM Chain ID:** 1612
   - **Token Symbol:** Pearl (test)
   - **VM Type:** Subnet-EVM
   - **RPC URL:** `https://subnets.avax.network/pearl/testnet/rpc`
   - **Explorer URL:** `https://subnets-test.avax.network/intersect`

3. Once added, you can use your wallet with the PEARL tokens on the Intersect Testnet.

You can also use the **dedicated RPC URL**:
```
https://testnet-pearl-c612f.avax-test.network/ext/bc/CcXVATAg76vM849mrPoTigwp48qhFiN9WCa51DBQXNGkBKZw7/rpc?token=3296aa3e491dd5d366815601cc95be7275cd293486b09fe082619750d7b38587
```

## Smart Contract Overview

The smart contracts handle decentralized project funding.

- **Project Creation:** Anyone can create a project by specifying a funding goal and deadline.
- **Funding a Project:** Users contribute PEARL tokens to a project's smart contract.
- **Withdraw Funds (Project Creators):** Creators can withdraw funds if the project meets its funding goal.
- **Refunds (Backers):** If the funding goal isn’t met, backers can withdraw their contributions.

## Testing

The dApp is deployed on Avalanche’s **Intersect Testnet** using **PEARL** as the test token.

- Use the faucet to obtain PEARL tokens.
- Fund and create projects using MetaMask on the testnet.
- Test interactions such as withdrawing funds and requesting refunds.

## Project Structure

- `contracts/` - Solidity smart contracts.
- `src/` - React frontend components.
- `scripts/` - Scripts to deploy smart contracts.

## Contributing

If you wish to contribute:

1. Fork the repo.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make changes and submit a pull request.

## Future Improvements

- Governance features (voting by backers).
- Enhanced user interface for improved user experience.
- Support for multiple cryptocurrencies for funding.
