---
path: find-nft-metadata
date: 2021-11-09T00:02:15.381Z
title: Find NFT metadata through Etherscan
description: Go to Etherscan, click Contract tab, under "Read Contract" query tokenURI
---
Let's use [this](https://etherscan.io/token/0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d?a=3958) NFT as an example.

Go to Contract tab, under "Read Contract" query tokenURI using the value 3958. You'll get this:
```
_string_ **:** ipfs://QmeSjSinHpPnmXmspMjwiXyN6zS4E9zccariGR3jxcaWtq/3958
```

Copy the string after "ipfs://" and use it to build a URL in this format: `https://ipfs.io/ipfs/(string you copied)`

https://ipfs.io/ipfs/QmeSjSinHpPnmXmspMjwiXyN6zS4E9zccariGR3jxcaWtq/3958

You'll see the metadata for this particular NFT. Look for the key "image" and do as you did earlier. Copy the string after "ipfs://" and use it to build a URL in this format: `https://ipfs.io/ipfs/(string you copied)`

https://ipfs.io/ipfs/Qmf5ZFdGJ59eudsmMy8zXdwNTd2yGNY2qrkszzQftgM32H

And here's the image for that NFT.