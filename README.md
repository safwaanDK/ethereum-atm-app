# Ethereum ATM Application - Readme

This is a simple Ethereum-based ATM application that allows users to deposit and withdraw Ether (ETH) from the deployed smart contract. Additionally, it provides functionality to check the account balance and transfer ownership of the contract to another address.

## Getting Started

To use the Ethereum ATM application, you need the following prerequisites:

1. MetaMask Wallet: Install the MetaMask browser extension for your web browser. Ensure you have an Ethereum account connected to MetaMask.

2. Node.js: Make sure you have Node.js installed on your system.

3. A supported web browser: The application is tested on modern web browsers like Chrome, Firefox, and Edge.

## Installation

1. Clone the repository to your local machine.

```
git clone <repository-url>
```

2. Navigate to the project directory.

```
cd ethereum-atm-app
```

3. Install the required dependencies using npm.

```
npm install
```

## Smart Contract

The smart contract code is written in Solidity and can be found in the `contracts/Assessment.sol` file. It includes the following functionalities:

- Deposit Ether into the contract.
- Withdraw Ether from the contract.
- Check the account balance of the contract.
- Get the current contract owner's address.
- Transfer ownership of the contract to another address.

The contract is deployed on the Ethereum blockchain using a development environment like Hardhat or Truffle.

## Frontend

The frontend code is built using React and can be found in the `src/components/HomePage.js` file. It interacts with the deployed smart contract using the ethers.js library to perform the following actions:

- Connect to MetaMask wallet and check user account status.
- Display account balance, contract owner, and provide buttons to deposit, withdraw, and transfer ownership.
- Deposit and withdraw Ether from the contract.
- Transfer ownership of the contract to another address.

## Deployment

Before running the application, you need to deploy the smart contract on the Ethereum blockchain. You can deploy it to a test network like Ropsten or Rinkeby or the Ethereum mainnet.

1. Modify the contract code in `contracts/Assessment.sol` as needed.
2. Deploy the contract using a development environment like Hardhat or Truffle.
3. Update the `contractAddress` variable in `src/components/HomePage.js` with the deployed contract's address.

## Running the Application

To run the Ethereum ATM application, execute the following command:

```
npm run dev
```

This will start the development server, and the application will be accessible at `http://localhost:3000/` in your web browser.

## Usage

1. Connect your MetaMask wallet to the application by clicking the "Connect" button.
2. Once connected, your account address will be displayed along with the current account balance and contract owner.
3. To deposit Ether, click the "Deposit 1 ETH" button.
4. To withdraw Ether, click the "Withdraw 1 ETH" button (assuming sufficient balance).
5. To transfer ownership of the contract, enter the new owner's address in the input field and click the "Transfer Ownership" button.

## Important Notes

- The application is for educational purposes and should not be used with real Ether or on the Ethereum mainnet without proper security audits.

- Ensure that your MetaMask wallet is set to the correct network (e.g., Ropsten or Rinkeby) where the contract is deployed.

- Transactions may take some time to be confirmed on the Ethereum blockchain. Always check transaction details on Etherscan or similar block explorers.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- The smart contract and frontend code are for demonstration purposes and based on simple functionalities.
- Thanks to the Ethereum community and OpenZeppelin for their contributions to the ecosystem.

## Disclaimer

This application is provided as-is without any warranties. Use it at your own risk. The authors are not responsible for any loss of funds or damages caused by using this application improperly.
