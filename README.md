# must-know-solidity-basics

## Pan cake swap Contracts in order

`Context` including the sender of the transaction and its data

`Ownable` (there is an account (an owner) that can be granted exclusive access)

`IBEP20` (interface of BEP20 functions)

`Address` (contains some utility functions for address)

`SafeMath` (a library to safely perform arthmetic operations)

`BEP20` (implementation of IBEP20)


## Solidity keywords understanding
`internal` (only contract and its derived contract can be used)

`external` (they can be called by other contracts and transactions)

`public` (can be called either internally or via messages [getter functions will automatically be created for these type of variables])

`private` (these are only visible to for the contract they are defined in and not in dervied contracts)

`view` (prevent modifying state of contract and functions within it)

`events` (an event is emitted, it stores the arguments passed in transaction logs)

`indexed` (it helps to filter logs on events by indexes [it only used with events])

`modifier` (it can be used to easily change the behaviour of functions. For example, they can automatically check a condition prior to executing the function.

`Modifiers` are inheritable properties of contracts and may be overridden by derived contracts.)

`using` (it's used for including a library within a contract in solidity)

`mapping` (These are used to store the data in the form of key-value pairs)

`pure` (Pure functions ensure that they not read or modify the state. A function can be declared as pure)

`Yul` (The language used for inline assembly in Solidity is called Yul)

`assembly` (Inline assembly is a way to access the Ethereum Virtual Machine at a low level. This bypasses several important safety features and checks of Solidity)


## Tokens Standards
`BEP20` (Its a developer-friendly token standard that allows anyone to deploy fungible digital currencies or tokens on Binance Smart Chain.)

`EIP-712` (Its for typed message signing. This standard allows wallets to display data in signing prompts in a structured and readable format)


## Important info useds in Standards
`chainId` (The EIP-155 chain id. Prevents a signature meant for one network, such as a testnet, from working on another, such as the mainnet.)

`salt` (A unique 32-byte value hardcoded into both the contract and the dApp meant as a last-resort means to distinguish the dApp from others)