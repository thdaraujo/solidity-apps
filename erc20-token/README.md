Create your own ERC20-token
----------------------------------

- Install metamask and go to test net (RINKEBY Test Network)
- Get some fake ether on a [faucet](https://faucet.rinkeby.io/)
- Post your account on social media and share on the faucet to get fake ether
- Edit contracts with remix
- Deploy with remix

# Implement the ERC20 token interface/standard

[ERC20 Token Standard](https://theethereum.wiki/w/index.php/ERC20_Token_Standard)

The `EIP20Interface` is an interface you must implement in order to create the token.

## Deploy token on the Network

- Login metamask
- Make sure you have some fake ether
- Remix -> Injected web3 on Rinkeby

Call create with the parameters [total supply, token name, decimals, symbol]:
9000, "BlockchainDev Token", 0, "BDT"

- Authorize transaction (and set gas amount)

- Go to etherscan and see the contract there
https://rinkeby.etherscan.io/token-search

- See contract
0xa005fe9141cddabed97fc38126bdc0c36598092e
https://rinkeby.etherscan.io/address/0xa005fe9141cddabed97fc38126bdc0c36598092e
