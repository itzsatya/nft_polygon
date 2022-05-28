
# Mint NFT Polygon

A git repository to mint nft on mumbai polygon network.


## How to mint NFT

First, clone repo and install node modules.

```bash
  git clone https://github.com/itzsatya/nft_polygon.git
  cd nft_polygon
  npm install
```

Now, compile the contracts and put it on the mumbai network.

```bash
  npx hardhat compile
  npx hardhat --network matic run scripts/deploy.js
```

And, note down the contract address to put on mint-nft.js file.

After that make a file like nft-metadata.json with data of ipfs and upload it to the ipfs to get the CID of json file.
(I used pinata.cloud to upload file to ipfs). Put CID to mint-nft.js file.

```bash
    node scripts/mint-nft.js
```

## Links

[Polygonscan link for deployed contract](https://mumbai.polygonscan.com/address/0xdb494d2f98074cb756610e3ac69e04c44fe0737b)

[Polygonscan link for deployed NFT](https://mumbai.polygonscan.com/tx/0x61698e06132bd156f896513a335779f8c5dcfda489afb75bebb68cafcec4503d)

[Opensea link to NFT](https://testnets.opensea.io/assets/mumbai/0x6e31503ff03aabd1a7347773febe9cff3bdfe4f1/1)
