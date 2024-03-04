# Opensea Lite(NFT Marketplace)

## Diagrammatic Brief

![nfts drawio](https://github.com/ichdamola/opensea-lite/assets/20647487/ecf26704-07a4-480a-8bc1-4417a02117b7)

## Technology Stack & Tools

| Technology                   | Description                      |
|------------------------------|----------------------------------|
| Solidity                     | Writing Smart Contracts          |
| Javascript                   | React & Testing                  |
| [Ethers](https://docs.ethers.io/v5/)   | Blockchain Interaction          |
| [Hardhat](https://hardhat.org/)        | Development Framework            |
| [Ipfs](https://ipfs.io/)               | Metadata Storage                 |
| [React Routers](https://v5.reactrouter.com/) | Navigational Components        |


## Requirements For Initial Setup
- Install [NodeJS](https://nodejs.org/en/), should work with any node version below 16.5.0
- Install [Hardhat](https://hardhat.org/)

# Setting Up

## 1. Clone/Download the Repository

## 2. Install Dependencies:
```bash
$ cd opensea-lite
$ npm install
```

## 3. Boot up Local Development Blockchain
```bash
$ cd nft_marketplace
$ npx hardhat node
```
## 4. Connect Development Blockchain Accounts to Metamask
- Copy the private key of the addresses and import it into Metamask.
- Connect your Metamask to the Hardhat blockchain, network 127.0.0.1:8545.
- If you haven't added Hardhat to the list of networks on your Metamask:
  1. Open up a browser, click the fox icon.
  2. Click the top center dropdown button listing all available networks, then click "Add Network."
  3. A form should pop up. Enter "Hardhat" for the "Network Name" field.
  4. Enter "http://127.0.0.1:8545" for the "New RPC URL" field.
  5. Enter "31337" for the chain ID. Click save.

## 5. Migrate Smart Contracts
```bash
$ npx hardhat run src/backend/scripts/deploy.js --network localhost
```

## 6. Run Tests
```bash
$ npx hardhat test
```
  ### Output
  <img width="776" alt="Screenshot 2024-03-04 at 15 04 34" src="https://github.com/ichdamola/opensea-lite/assets/20647487/c0179f52-cbe4-4d56-8952-59f5fcf832b4">

## 7. Launch Frontend
```bash
$ npm run start
```

## License

MIT
