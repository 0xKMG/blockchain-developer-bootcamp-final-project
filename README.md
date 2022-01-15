# Final project - Simple Staking

## Deployed version url:

http://KMGwei.github.io/blockchain-developer-bootcamp-final-project 

## How to run this project locally:

### Prerequisites

- Node.js >= v14
- Truffle and Ganache
- download or clone the repository from "https://github.com/KMGwei/blockchain-developer-bootcamp-final-project"

### Contracts

- Run `npm i` in project root to install smart contract dependencies
- Run local testnet in port `7545` with an Ethereum client, e.g. Ganache
- `truffle migrate --reset`
- Run tests in Truffle `truffle test`

### Frontend

- `npm run start`
- Open `http://localhost:3000`

## How to Interact with the DApp
There are 2 ways to interact with this DApp.

### Interact through publicly deployed web interface

http://KMGwei.github.io/blockchain-developer-bootcamp-final-project

### Interact through local network

Run `npm install` to install all the dependencies in the package.json file
Launch the user interface via port: 3000 by running the following command in the root directory `npm run start`
Access the user interface via http://localhost:3000
If you do not have Metamask browser extension, install Metamask in your browser. Connect your Metamask wallet and start interacting with the app.

## Screencast link

https://youtu.be/tdFkPFzoWOY


## Public Ethereum wallet for certification:

`0xf7232E584fC544d6A5F9A8F050111E2fB5bACFad`

## Project description

Simple Staking 

This DApp provides an ERC20 token (Mock Tether Token) deposit and withdrawal services to users. The user's deposit will earn rewards (and airdrop) at the will of the Bank owner. Please note that the issue token function can only be accessed through the terminal in a local environment, frontend functionality will be available in the future. 

The DApp uses Openzeppelin ERC20 standard to build the Mock Tether Token and RWD Token. 

The contract is deployed on the Ropsten testnet at 

0x7e35C07C95263985a5E44639FdB1Bf332D1EfA85


## Simple workflow

1. Enter the website
2. Login with Metamask
3. Enter the amount to Stake
4. Confirm the amount with Metamask (smart contract call)
5. Staking Amount Updated on the Frontend
6. Withdraw the amount at anytime 


## Directory structure

Key files and folders structures are as below:
```
blockchain-developer-bootcamp-final-project-(root directory)
+-- migrations
|   +-- 1_initial_migration.js
|   +-- 2_deploy_contracts.js 
|
+-- public
|
+-- src
|   +-- truffle_abis
|   +-- Component
|   |   +-- App.js
|   |   +-- Main.js
|   |   +-- Navbar.js
|   |   +-- ParticleSettings.js
|   |
|   +-- contracts
|   |   +-- Migrations.sol
|   |   +-- DencentralBank.sol  
|   |   +-- RWD.sol    
|   |   +-- Tether.sol      
|   |
|
+-- test
|   +-- simplestaking.test.js    
+-- truffle-config.js
+-- issue-tokens.js
+-- package.json
+-- .env.example
+-- avoiding_common_attacks.md
+-- design_pattern_decisions.md
+-- deployed_address.txt
```

## Environment variables (not needed for running project locally)

```
ROPSTEN_INFURA_PROJECT_ID=
ROPSTEN_MNEMONIC=
```

## TODO features

- Issue Token Function - Frontend
- User getting rewards based on how long they have staked
