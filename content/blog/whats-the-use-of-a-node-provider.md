---
path: Node-provider
date: 2021-11-06T22:25:56.253Z
title: What's the use of a Node Provider?
description: Node Providers free users from setting up and manage their own blockchain node
---
There’s no way to access the information on a blockchain without using a node. We can say that a node is to the Blockchain what the browser is to the internet.

There’s no way to access the information on a blockchain without using a node. We can say that a node is to the Blockchain what the browser is to the internet.
There’s no way to access the information on a blockchain without using a node. We can say that a node is to the Blockchain what the browser is to the internet.

There are two types of nodes:
- light node
- full node

If you're testing a dapp on the local computer, Hardhat/Truffle create for you a local node.

But when you're deploying the dapp to the main net or even to the test net you need to use a Node Provider (running your own node is a headache!)

## What's a Node Provider?

It's a service that provides blockchain nodes freeing users from setting up and manage their own blockchain node.

Popular node providers:
- Infura
- Alchemy


### Why do you need to use a Node Provider in your dApp?

Two simple reasons:

1. Deploying your smart contract to the main net or test net is done via a transaction to the blockchain. This can only happen if you have access to a node. That means running your own node, or sending your transaction to a provider.
2. Your dapp will likely pull data from the Blockchain. And that it's also done via a node.

This is why node providers are important.
