Degen Token

For this task we will create a ERC20 token and deploy it on the Avalanche network for Degen Gaming. The smart contract should have the following functionality:

Minting new tokens: The platform should be able to create new tokens and distribute them to players as rewards. Only the owner can mint tokens. Transferring tokens: Players should be able to transfer their tokens to others. Redeeming tokens: Players should be able to redeem their tokens for items in the in-game store. Checking token balance: Players should be able to check their token balance at any time. Burning tokens: Anyone should be able to burn tokens, that they own, that are no longer needed. Description This is a smart contract written in Solidity programming language for Ethereum blockchain. It extends an ERC20 token standard with the Ownable module from OpenZeppelin Contracts for access control.

Here's a brief explanation of what each part does:

The pragma statement sets the version of Solidity compiler this contract is compatible with. It means it can only be compiled with versions of compiler starting from 0.8.20 up to 0.8.20 (inclusive).

The import statements include OpenZeppelin Contracts' ERC20 and Ownable modules which give it a standard ERC20 token interface and access control features respectively.

The contract 'DegenToken' inherits from both ERC20 and Ownable contracts. It is a decentralized digital currency with custom functionalities.

The contract has several events for logging transactions for transparency and auditability.

It defines a struct 'Item' for tracking quantity and price of items in a trade or redemption.

It also defines a struct 'Trade' for recording information about trades.

It uses mappings (like Python's dictionaries) for items and trades with string keys for item names and uint256 keys for trade IDs.

The contract constructor initializes ERC20 token with a name 'Degen' and symbol 'DGN', and sets the initial owner of the contract using Ownable module.

The contract includes several custom functions for minting (creating) new tokens, burning (removing) tokens from an account's balance, transferring tokens between accounts, redeeming tokens (removing tokens from balance of an account), listing an item for trade or redemption, creating a trade, completing a trade, retrieving trade information, and checking an account's balance.

The modifier 'onlyOwner' is used for restricting access to certain functions to contract owner only.
