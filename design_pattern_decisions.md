# Design patterns used

## Inter-Contract Execution (Calling functions in external contracts)

My project has 3 contracts - DecentralBank (the main contract), which embeds within it an instance of the RWD and Tether contract. The transferFrom and transfer funcction from both token contracts are called in the main contract. 


## Inheritance and Interfaces

- Both Tether.sol and RWD.sol inherits the OpenZeppelin `ERC20` contract to enable functions such as total supply, balance of, transfer and approve. 