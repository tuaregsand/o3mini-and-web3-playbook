```markdown
# O3-Mini-High Prompt Directory for Web3 & Solana Development

This repository contains a curated list of prompt templates designed to help you harness the power of O3-Mini-High for Web3 and Solana development (with a focus on Rust and Anchor). Use these templates as a starting point for generating code, debugging, testing, and automating various tasks in your development workflow.

---

## Table of Contents
- [Environment Setup Prompts](#environment-setup-prompts)
  - [Prompt 1.1: Setup Development Environment](#prompt-11-setup-development-environment)
  - [Prompt 1.2: Configure Solana CLI](#prompt-12-configure-solana-cli)
- [Code Generation & Smart Contract Prompts](#code-generation--smart-contract-prompts)
  - [Prompt 2.1: Generate a Solana Escrow Program (Anchor & Rust)](#prompt-21-generate-a-solana-escrow-program-anchor--rust)
  - [Prompt 2.2: NFT Minting Contract](#prompt-22-nft-minting-contract)
- [Off-Chain API Integration Prompts](#off-chain-api-integration-prompts)
  - [Prompt 3.1: Fetch Wallet Balance with Solana RPC (Rust)](#prompt-31-fetch-wallet-balance-with-solana-rpc-rust)
  - [Prompt 3.2: REST API Outline for Solana dApp](#prompt-32-rest-api-outline-for-solana-dapp)
- [Debugging and Code Review Prompts](#debugging-and-code-review-prompts)
  - [Prompt 4.1: Debug 'AccountBorrowFailed' Error](#prompt-41-debug-accountborrowfailed-error)
  - [Prompt 4.2: Code Review & Security Audit for a Solana Program](#prompt-42-code-review--security-audit-for-a-solana-program)
- [Testing and Simulation Prompts](#testing-and-simulation-prompts)
  - [Prompt 5.1: Generate Anchor Test for Escrow Failure](#prompt-51-generate-anchor-test-for-escrow-failure)
  - [Prompt 5.2: Simulate On-Chain Event Analysis](#prompt-52-simulate-on-chain-event-analysis)
- [Bot and Automation Development Prompts](#bot-and-automation-development-prompts)
  - [Prompt 6.1: Build a Solana Dev Assistant Chatbot](#prompt-61-build-a-solana-dev-assistant-chatbot)
  - [Prompt 6.2: On-Chain Event Notification Bot](#prompt-62-on-chain-event-notification-bot)
- [How to Use These Prompts](#how-to-use-these-prompts)

---

## Environment Setup Prompts

### Prompt 1.1: Setup Development Environment
**Description:** Generate a detailed guide for installing and configuring all tools needed for Solana development.

**Prompt Text:**
```plaintext
Generate a step-by-step guide for setting up a Solana development environment. Include instructions for installing Rust (via rustup), the Solana CLI (including solana-test-validator), and the Anchor framework. Provide command examples, configuration tips (such as setting the correct network URL and keypair locations), and best practices for organizing your project structure.
```

**Tags:** `#setup` `#environment` `#Rust` `#Solana` `#Anchor`

---

### Prompt 1.2: Configure Solana CLI
**Description:** Create a concise prompt to configure the Solana CLI for devnet usage and keypair setup.

**Prompt Text:**
```plaintext
Provide clear commands to configure the Solana CLI to connect to devnet. Include commands for setting the network URL (e.g., 'solana config set --url https://api.devnet.solana.com'), generating a new keypair if none exists, and verifying the configuration.
```

**Tags:** `#Solana` `#CLI` `#configuration`

---

## Code Generation & Smart Contract Prompts

### Prompt 2.1: Generate a Solana Escrow Program (Anchor & Rust)
**Description:** Use O3-Mini-High to generate a complete smart contract that implements an escrow mechanism using Anchor.

**Prompt Text:**
```plaintext
Write an Anchor-based Solana smart contract in Rust that implements a token escrow. The contract should include:
1. An initializer that deposits tokens into escrow.
2. A function for a counterparty to deposit tokens, which then triggers the token swap.
Include inline comments explaining each step and account validation checks.
```

**Tags:** `#SmartContract` `#Escrow` `#Rust` `#Anchor` `#Solana`

---

### Prompt 2.2: NFT Minting Contract
**Description:** Generate a prompt to create an NFT minting program on Solana using Anchor.

**Prompt Text:**
```plaintext
Generate a Solana smart contract in Rust using the Anchor framework that implements NFT minting. Define the necessary account structures, include functions to mint an NFT, and handle metadata appropriately. Make sure to add inline comments and usage examples.
```

**Tags:** `#NFT` `#Minting` `#Solana` `#Rust` `#Anchor`

---

## Off-Chain API Integration Prompts

### Prompt 3.1: Fetch Wallet Balance with Solana RPC (Rust)
**Description:** Create a Rust function that uses the Solana RPC API to get a wallet’s SOL and token balances.

**Prompt Text:**
```plaintext
Write a Rust function that uses 'solana_client::RpcClient' to fetch the SOL balance and list all SPL token balances for a given wallet address (Pubkey). Ensure that the code includes proper error handling and clear inline comments.
```

**Tags:** `#API` `#Solana` `#Rust` `#RPC` `#Wallet`

---

### Prompt 3.2: REST API Outline for Solana dApp
**Description:** Generate an outline for a RESTful API that a Solana dApp could use.

**Prompt Text:**
```plaintext
Design a REST API for a Solana-based dApp. Outline endpoints such as:
- GET /balance: Returns the SOL balance for a given wallet.
- POST /transaction: Submits a transaction.
- GET /transaction-status: Checks the status of a submitted transaction.
For each endpoint, provide a brief description along with sample JSON request and response schemas.
```

**Tags:** `#RESTAPI` `#Web3` `#Solana` `#Design`

---

## Debugging and Code Review Prompts

### Prompt 4.1: Debug 'AccountBorrowFailed' Error
**Description:** Ask the model to analyze a snippet of Rust code that triggers an 'AccountBorrowFailed' error.

**Prompt Text:**
```plaintext
Analyze the following Rust code from a Solana program that results in an 'AccountBorrowFailed' error. Identify potential causes of the error and provide a corrected version of the code with an explanation of the changes.
[Insert Code Snippet Here]
```

**Tags:** `#Debugging` `#Error` `#Rust` `#Solana`

---

### Prompt 4.2: Code Review & Security Audit for a Solana Program
**Description:** Request an in-depth code review focusing on security, performance, and style.

**Prompt Text:**
```plaintext
Review the following Solana program code (in Rust) for potential issues. Focus on:
- Security vulnerabilities (e.g., missing signer checks or unchecked arithmetic operations).
- Performance improvements.
- Code clarity and style.
List any issues found along with suggestions for corrections.
[Insert Code Snippet Here]
```

**Tags:** `#CodeReview` `#Security` `#Solana` `#Rust`

---

## Testing and Simulation Prompts

### Prompt 5.1: Generate Anchor Test for Escrow Failure
**Description:** Produce an Anchor test case that simulates a failure in an escrow scenario.

**Prompt Text:**
```plaintext
Write an Anchor test in Rust that simulates an unauthorized withdrawal attempt from an escrow program. The test should set up the necessary accounts, attempt the withdrawal, and assert that the transaction fails with the expected error.
```

**Tags:** `#Testing` `#Anchor` `#Solana` `#Escrow` `#Rust`

---

### Prompt 5.2: Simulate On-Chain Event Analysis
**Description:** Create a prompt for generating a natural-language report summarizing a significant on-chain event.

**Prompt Text:**
```plaintext
Draft a report analyzing a large token transfer event on Solana. The report should include:
- Involved accounts and the amount transferred.
- Potential reasons for the event (e.g., liquidation, large trade).
- A summary of its implications.
Use any provided log snippets as context.
```

**Tags:** `#Simulation` `#OnChainAnalysis` `#Report` `#Solana`

---

## Bot and Automation Development Prompts

### Prompt 6.1: Build a Solana Dev Assistant Chatbot
**Description:** Generate code for a Discord bot that assists developers with Solana-related queries.

**Prompt Text:**
```plaintext
Create a basic Node.js implementation for a Discord chatbot that provides Solana development assistance. The bot should:
- Respond to commands like '!balance <wallet_address>' by fetching and displaying the wallet balance via Solana RPC.
- Provide development tips on command '!help'.
Include example code for setting up the bot, integrating with Solana's API, and handling user commands.
```

**Tags:** `#Bot` `#Discord` `#Solana` `#Web3` `#Node.js`

---

### Prompt 6.2: On-Chain Event Notification Bot
**Description:** Develop a script that monitors on-chain events and sends notifications.

**Prompt Text:**
```plaintext
Write a script that monitors Solana on-chain events using either WebSocket subscriptions or periodic RPC polling. When a significant event (like a large liquidation or token transfer) is detected, the script should generate a concise, human-readable alert and send it to a Slack or Telegram channel. Ensure to include error handling and performance optimizations.
```

**Tags:** `#Bot` `#OnChain` `#Notification` `#Solana` `#Automation`

---

## How to Use These Prompts

1. **Copy and Customize:** Copy the prompt text into your preferred environment or directly into the O3-Mini-High interface. Adjust details—such as inserting code snippets or endpoint names—to match your project context.
2. **Iterate:** Refine the prompt based on initial outputs. Add more context or specific instructions if necessary.
3. **Integrate:** Use the generated code or documentation as a foundation for your smart contract, API integration, or automation script. Always test and validate the outputs.
4. **Share:** Contribute back to the community by adding your improved prompts to this directory or your team’s documentation.

---
```
