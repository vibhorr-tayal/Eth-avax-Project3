# Eth-avax-Project3
# Vibhor Token

## Introduction

This repository contains the Solidity smart contract code for the token, an ERC-20 compatible token designed for various purposes. These tokens can be used for transactions, rewards, and other activities within an ecosystem.

## Contract Details

The `Token.sol` file contains the source code for the token contract. Here are the key details of the contract:

- Token Name: Vibhor
- Token Symbol: Vib
- Total Supply: 0 (initially)

The contract includes standard ERC-20 functions such as `balanceOf` and `transfer`. It also includes functionalities for minting and burning tokens, accessible only by the contract owner.

The contract owner has special privileges and is the only address allowed to mint new tokens. Other addresses can interact with the contract by transferring tokens and burning their own tokens.

### Execution of the Program

Follow these steps to To deploy the token contract to the local Hardhat test network using Remix Connect Localhost

- Clone the repository and install its dependencies:

```sh
git clone https://github.com/RIDAMSINHA/INTERACTING-AND-DEPLOYING-ON-LOCAL-NETWORK.git
cd INTERACTING-AND-DEPLOYING-ON-LOCAL-NETWORK
npm install
```

* Install the `@remix-project/remixd` dependency to connect Remix IDE:

```sh
npm install -g @remix-project/remixd
```

- Run the following command in the terminal to connect Remix IDE to the Hardhat local host:

```sh
remixd -s ./ --remix-ide https://remix.ethereum.org
```

- Open a new terminal and start Hardhat's testing network:

```sh
npx hardhat node
```

- Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

- In the file explorer in the workspace, select "localhost" to connect to the local Hardhat network.

- Rewrite the `Token.sol` file in the contracts directory with your RUK token contract code.

- Compile the contract in the Remix IDE.

- In the deploy section of Remix, select the environment as "Dev-Hardhat Provider".

- Deploy your contract on the local Hardhat network using the deploy button in Remix.

- Confirm the deployment transaction in Remix.

- Wait for the deployment transaction to be confirmed on the local Hardhat network.

- Once the contract is deployed, you will see the contract address in the Remix console. Make note of this address for future interactions.

## Interacting with the Contract using Remix with Hardhat Provider

After deploying the RUK token contract to the local Hardhat test network, you can interact with the contract using Remix with Hardhat provider. Here are the steps to get started:

- Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

- In the "File Explorer" section, locate the `Token.sol` file and open it.

- In the "Deployed Contracts" section, click on the contract named `Token`.

- In the "At Address" input field, enter the contract address obtained during deployment.

- Click the "At Address" button to load the contract instance.

- You can now interact with the RUK token contract through the provided functions.

  - Use the `balanceOf` function to check the token balance of a specific address.
  - Use the `transfer` function to send RUK tokens from your address to another address.
  - Use the `mint` function (accessible only to the contract owner) to mint new tokens.

- Use the `burn` function to burn a specific amount of your tokens.

* Set the required parameters for each function and click the corresponding button to execute the transaction.

* Confirm the transaction details and sign the transaction in Remix.

* Wait for the transaction to be confirmed on the local Hardhat network.

* You can view the transaction status and emitted events in the Remix console.

## Authors

This project is authored by Vibhor Tayal.

## License

The SimpleContract project is licensed under the MIT License, granting you the flexibility to modify and distribute the code as needed.
