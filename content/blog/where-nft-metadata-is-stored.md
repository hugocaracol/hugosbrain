---
path: Where NFT metadata is stored
date: 2021-11-05T23:47:47.666Z
title: Where NFT metadata is stored
description: Regarding data storage (baseURI and tokenURI), the best practice is
  to store it on an immutable decentralized network like IPFS or Arweave
---

This is a destillation of a [tweet](https://twitter.com/dabit3/status/1456399715646513153) from Nader Babit.

Let's talk about NFT metadata on EVM (Ethereum Virtual Machine).

The most popular standard for creating NFTs on Ethereum is ERC721. Each ERC721 token is unique, which is not the case of ERC20 tokens.

*(Important: In the end of this post there's a section named "Find NFT metadata through Etherscan" where I show the steps to find an image of an NFT given the contract address.)*

## Concerns about data storage

### Important properties

Three of the key properties of ERC721 tokens are:

#### - tokenId

You can mint multiple tokens in a single contract, each one having a unique TokenId.

Example: One tokenId of BoredApeYachtClub NFTs is [3958](https://etherscan.io/token/0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d?a=3958).


#### - baseURI

Defines the base for the tokenURI.

Example: For the previous tokenID (3958), the baseURI is the string `ipfs://QmeSjSinHpPnmXmspMjwiXyN6zS4E9zccariGR3jxcaWtq/`


#### - tokenURI

The tokenURI defines the metadata for the token.

Example: For the tokenId 3958, the tokenURI is the string `ipfs://QmeSjSinHpPnmXmspMjwiXyN6zS4E9zccariGR3jxcaWtq/3958`


### Data Storage best practice

Regarding data storage (baseURI and tokenURI), the best practice is to store it on an immutable decentralized network like IPFS or Arweave, or written into the NFT itself using something like SVG (One example is the [developer_dao](https://etherscan.io/address/0x25ed58c027921e14d86380ea2646e3a1b5c55a8b) token.

This data should **never** be stored on a centralized hosting server like S3 or other alike.
This should never be done because the data would not be immutable, *if* anyone who runs those servers can update the data **or** if someone stopped paying the bill for this service.


