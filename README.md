# Simple AI NFT Generator
The Simple AI NFT Generator utilizes A.I. to generate unique artwork and create non-fungible tokens (NFTs) on the blockchain.

## Features
* Connects with MetaMask wallet
* Generates artwork using AI image generator - Hugging Face's stable diffusion model
* Uploads artwork to IPFS
* Mints NFTs using Open Zeppelin framework to interact with ERC721


## How it Works
* Users can connect their MetaMask wallet to the app, which allows them to mint NFTs using Ether.
* The app includes a form for user input, which captures information about the desired AI-generated artwork.
* The user input is sent to the Hugging Face API, which uses its stable diffusion model to generate a unique image.
* The generated image is uploaded to IPFS and the Open Zeppelin framework is used to mint a new NFT on the blockchain.
* The user can then view their NFT and interact with it on the Ethereum blockchain.

## Technology Stack & Tools

- Solidity (Writing Smart Contracts & Tests)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.io/v5/) (Blockchain Interaction)
- [React.js](https://reactjs.org/) (Frontend Framework)
- [NFT.Storage](https://nft.storage/) (Connection to IPFS)
- [Hugging Face](https://huggingface.co/) (AI Models)

## Requirements For Initial Setup
- Install [NodeJS](https://nodejs.org/en/)

## Setting Up
### 1. Clone/Download the Repository

### 2. Install Dependencies:
`$ npm install`

### 3. Setup .env file:
Before running any scripts, you'll want to create a .env file with the following values (see .env.example):

- **REACT_APP_HUGGING_FACE_API_KEY=""**
- **REACT_APP_NFT_STORAGE_API_KEY=""**

You'll need to create an account on [Hugging Face](https://huggingface.co/), visit your profile settings, and create a read access token. 

You'll also need to create an account on [NFT.Storage](https://nft.storage/), and create a new API key.

### 4. Run tests
`$ npx hardhat test`

### 5. Start Hardhat node
`$ npx hardhat node`

### 6. Run deployment script
In a separate terminal execute:
`$ npx hardhat run ./scripts/deploy.js --network localhost`

### 7. Start frontend
`$ npm run start`


![Animated GIF](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZmE3ZWQ0ODQwZGViY2E1MGJiNjhhMDYxOTBiYmYwY2ZmYTNjOTJkZCZjdD1n/Y83o2JkdkXM9rYMJ3P/giphy.gif)
