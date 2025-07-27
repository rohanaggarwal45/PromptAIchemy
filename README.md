# AI Prompt Marketplace - Smart Contracts

This module contains the smart contracts for the AI Prompt Marketplace, built using Solidity and Hardhat.

## Overview

The smart contract module includes:
- `PromptNFT.sol`: Main contract for minting and managing AI prompt NFTs
- Test suite for contract verification
- Deployment scripts
- Hardhat configuration

## Features

- Mint AI prompts as NFTs with metadata
- Support for both image and text prompts
- ERC2981 royalty standard implementation
- Ownership verification
- Event emission for minting and royalty payments

## Prerequisites

- Node.js (v14 or later)
- npm or yarn
- MetaMask or another Ethereum wallet

## Installation

1. Install Node.js from https://nodejs.org/
2. Install the dependencies:
```bash
npm install
```

## Usage

1. Compile the contracts:
```bash
npm run compile
```

2. Run tests:
```bash
npm test
```

3. Start a local blockchain:
```bash
npm run node
```

4. Deploy contracts (in a new terminal):
```bash
npm run deploy:local
```

## Contract Details

### PromptNFT

The main contract inherits from:
- ERC721: Base NFT functionality
- ERC721URIStorage: Metadata storage
- ERC2981: Royalty standard
- Ownable: Access control

Key functions:
- `mintPrompt`: Create a new prompt NFT
- `getPromptMetadata`: Retrieve prompt details
- `verifyPromptOwnership`: Check prompt ownership
- Built-in royalty support with customizable fees

## Testing

The test suite covers:
- Minting functionality
- Royalty calculations
- Ownership verification
- Error cases

## License

MIT
