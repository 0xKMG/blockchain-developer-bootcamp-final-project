Avoiding Common Attacks

// 1. SWC-103 - avoiding floating pragma, favoring a locked (specific) version of the solidity compiler ------- Simple Staking uses "pragma solidity 0.8.0" specifically, as per the recommendations from SWC-103 - avoiding floating pragma, favoring a locked (specific) version of the solidity compiler ------- Also using a specific solc compiler version configuration in the "compilers" section on truffle-config.js

// 3. SWC-100 Function Default Visibility ------- Simple Staking has made conscious decisions on which visibility type is appropriate for every function on the PearlZZExchange & PearlZZToken smart contract, ------- thereby dramatically reducing the attack surface.