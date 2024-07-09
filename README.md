# Polygon-mod-1

## NFT Collection README

## Overview
This repository contains scripts and contracts to facilitate the creation, deployment, and management of an NFT collection. The collection is generated using DALLE 2 or Midjourney, stored on IPFS using pinata.cloud, and deployed on the Goerli Ethereum Testnet as ERC721 or ERC1155 tokens. Additionally, scripts are provided to handle batch minting, transferring NFTs between Ethereum and Polygon Mumbai using the FxPortal Bridge, and testing functionalities.

## Requirements
- Node.js (v14 or above)
- Hardhat (v2.x or above)
- Metamask or other Ethereum wallet for testnets
- Pinata.cloud API keys for IPFS storage

## Setup
1. Clone this repository:
   ```
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Configure environment variables:
   - Create a `.env` file based on `.env.example` and fill in necessary details such as API keys, wallet mnemonic, and network configurations.

## Steps to Deploy NFT Collection

### Step 1: Generate NFT Images
- Use DALLE 2 or Midjourney to generate a 5-item collection of NFT images.

### Step 2: Store Items on IPFS
- Upload each generated image to IPFS using pinata.cloud for decentralized storage.

### Step 3: Deploy ERC721/ERC1155 Contract
- Deploy the contract to the Goerli Ethereum Testnet. Ensure the contract includes a `promptDescription` function that returns the prompt used for image generation.

### Step 4: Map Your NFT Collection (Optional)
- Use the Polygon network token mapper to map your NFT collection for improved visualization and interoperability.

### Step 5: Batch Mint NFTs
- Execute the provided Hardhat script (`mint-nfts.js`) to batch mint all NFTs. Adjust parameters as necessary for ERC721 or ERC1155 standards.

### Step 6: Batch Transfer to Polygon Mumbai
- Utilize the Hardhat script (`transfer-nfts.js`) to batch transfer all minted NFTs from Ethereum to Polygon Mumbai using the FxPortal Bridge.

### Step 7: Approve and Deposit NFTs
- Approve the NFTs to be transferred using Metamask or similar wallet.
- Deposit the NFTs to the FxPortal Bridge for cross-chain transfer.

### Step 8: Test BalanceOf on Polygon Mumbai
- Run tests using the Hardhat script (`test-balance.js`) to ensure correct balances of NFTs on Polygon Mumbai after transfer.

## Additional Notes
- Ensure all environment variables and configurations are correctly set before deploying or testing.
- For detailed instructions and parameter adjustments, refer to individual script comments and the Hardhat documentation.

---

Feel free to customize this README with more specific details or additional instructions based on your project's requirements and preferences.
- - -
