# Eth-avaxinterproj-4

## DegenToken
- DegenToken is an ERC20 token deployed on the Avalanche Fuji Test Network.
- This token includes a simple store where users can redeem their tokens for store items.
- The token also includes basic functionalities such as minting, burning, and transferring tokens.

# Description
This contract is written in Solidity language, a programming language used for developing smart contracts on the Ethereum blockchain. In smart contract first we imported 3 libraries ERC20, Ownable, ERC@)Burnable. The DegenToken contract is an ERC20 token with additional functionality for membership tiers and token burning. Players can purchase tokens and be added to a minting queue managed by the owner. Tokens can be transferred, redeemed for various membership levels by burning specific amounts, and balance checks can be performed by users. The contract also allows the owner to burn tokens from any address for gas management purposes.

# Overview
- DegenToken is implemented using the OpenZeppelin ERC20 contract. The contract includes the following features:

- Minting: Only the contract owner can mint new tokens.
- Burning: Any token holder can burn their tokens.
- Store: A list of items that can be redeemed using the tokens. Only the owner can add new items to the store.
- Contract Details
- Token Name: Degen
- Token Symbol: DGN
- Initial Supply: 0 DGN
# Functions
- Owner-Only Functions
- mint(address to, uint256 amount)

1. Mints new tokens and assigns them to the specified address.
- Only callable by the contract owner.
- addStoreItem(string memory itemName, uint256 price)

2. Adds a new item to the store with a specified name and price.
- Only callable by the contract owner.
- Public Functions
- redeemTokens(uint256 itemId)

3. Redeems tokens for a store item. The token price of the item is transferred from the caller to the owner.
- Callable by any user with sufficient token balance.
- burn(uint256 amount)



# To interact with the contract using Remix:

- Open Remix: Go to Remix IDE.
- Load Contract: Copy and paste the contract code into a new file in Remix.
- Install OpenZeppelin: Ensure you have imported the OpenZeppelin ERC20 contract.
- Compile Contract: Use the Solidity compiler to compile the contract.
- Deploy Contract: Deploy the contract using the "Injected Web3" environment in Remix and connect your wallet configured for the Avalanche Fuji Test Network.
- This README provides a clear and concise overview of your DegenToken project without including the actual contract code, ensuring it is user-friendly and easy to understand.

  ## Author
  Abhinav Singh

  ## Licence

  
