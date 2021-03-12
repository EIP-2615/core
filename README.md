# EIP-2615 Core

> EIP-2615 Rental and Mortgage functions for NFTs

This is the entry-point to learn more and participate in the EIP-2615 community efforts. One good place to begin is the [official EIP-2615](https://eips.ethereum.org/EIPS/eip-2615).

## Current Status

There are currently two competing ideas:

1) The original EIP-2615 proposes a new token standard that adds additional functions on top of ERC721 (i.e. you would need to make "new" NFTs that have both ERC721 and EIP-2615 functions). Existing ERC721 tokens would not be able to take advantage of these new functions. New tokens must be created.

2) A new registry contract that keeps track of "right of use" in order to augment existing ERC721 tokens. There is no token migration required, but if someone wants to check who has the "right of use", they would need to refer to a separate smart contract (external from the originally deployed ERC721 contract), meaning dapps that interact w/ the token would need to manage deploying and interacting with two separate contracts.

Both @kohshiba and @wighawag have created PoCs for both of these (see links below).

## Links

### Official

- [Official EIP](https://eips.ethereum.org/EIPS/eip-2615)
- [Original Discussion Issue](https://github.com/ethereum/EIPs/issues/2616)
- [Working Group Announcement Blog Post](https://medium.com/blockchain-game-alliance/nft-rental-and-mortgage-eip-2615-working-group-48b9bf8b164e)

### Implementations

- [@kohshiba's Original PoC](https://github.com/kohshiba/ERC-X)
- [@wighawag's Lease PoC](https://github.com/wighawag/erc721-lease)
- [@wighawag's Old Registry PoC](https://github.com/wighawag/erc721-users)
