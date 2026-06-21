# AntChain MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/antchain)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/antchain-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/antchain-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Alibaba's enterprise blockchain API hub — query blocks, transactions, smart contracts, and accounts on AntChain BaaS.

## Description
Connect your **AntChain (蚂蚁链)** BaaS platform account to any AI agent and gain complete visibility and control over your enterprise blockchain operations through natural conversation. AntChain is Alibaba Group's blockchain-as-a-service platform, designed for consortium chains, enterprise smart contracts, and secure decentralized applications.

### What you can do

- **Block Exploration** — Query detailed information about any block by height or hash, including transaction counts and timestamps
- **Transaction Tracking** — Inspect individual transactions by hash or ID, verifying status, gas consumption, and execution results
- **Smart Contract Management** — Deploy new contracts, invoke contract methods, and query contract metadata and ABIs
- **Account Inspection** — Check account balances, nonce values, and metadata for any wallet address on the chain
- **Network Monitoring** — View network topology, node status, consensus state, and chain health metrics
- **Chain Discovery** — List all blockchain networks available to your organization with their configurations
- **Recent Activity** — Monitor the latest transactions and network activity in real-time

### How it works

1. Subscribe to this server
2. Enter your AntChain Access Key and Secret Key
3. Start querying your blockchain networks from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your blockchain operations center, handling contract deployment, transaction verification, and network monitoring without complex CLI tools.

### Who is this for?

- **Blockchain Developers** — Deploy and interact with smart contracts directly from your IDE using natural language
- **Enterprise Ops** — Monitor consortium chain health, node status, and network metrics through conversational queries
- **Auditors & Compliance** — Verify transaction finality, inspect account balances, and audit contract executions
- **Product Teams** — Query blockchain data for dApps without writing boilerplate API integration code


## Available Tools
- **deploy_contract**: Requires the contract bytecode (compiled bytecode in hex format) and optionally the ABI (Application Binary Interface) for interaction. Returns the deployed contract address and deployment transaction details. The contract will be available under the specified name.

Deploy a smart contract on AntChain
- **get_chain_list**: Returns chain IDs, names, creation dates, status, and basic configuration. Use this to discover which blockchains you have access to before performing operations.

List all available blockchain networks in your AntChain account
- **invoke_contract**: Provide the contract name, method name, and any required arguments. Returns the execution result including return values, gas consumption, and transaction status. Use this to interact with deployed contracts.

Invoke a smart contract method on AntChain
- **query_account_balance**: Returns the available balance and any locked/pending amounts. Useful for checking if an account has sufficient funds for transactions or contract interactions.

Query account balance on AntChain
- **query_account**: Use this to inspect account state and activity.

Query account information on AntChain
- **query_block**: Returns block metadata including timestamp, transaction count, hash, and previous block reference. Use either blockHeight or blockHash to identify the block.

Query block details from an AntChain blockchain
- **query_contract**: Useful for inspecting contract configuration before invocation.

Query smart contract information on AntChain
- **query_latest_transactions**: Useful for monitoring network activity, auditing recent transactions, or getting a snapshot of current blockchain operations. Returns a list of recent transactions with their status and metadata.

Query the latest transactions on an AntChain blockchain
- **query_network_info**: Useful for monitoring blockchain infrastructure health.

Query blockchain network information on AntChain
- **query_transaction**: Returns transaction status, sender, receiver, gas used, block inclusion, and execution result. Useful for verifying transaction finality and inspecting transaction details.

Query a transaction on AntChain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AntChain** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest 5 transactions on my default AntChain network."

**🤖 AI Agent:**
> 📋 Here are the 5 most recent transactions on chain 'default'. The latest transaction (hash: 0xabc123...) was successful, transferring assets between accounts. Block height: 45678. Gas used: 21000. All 5 transactions show successful execution with varying gas costs.

---

**👤 You:**
> "What's the balance of account 0x742d35Cc6634C0532925a3b844Bc9e7595e0bFa8?"

**🤖 AI Agent:**
> 💰 Account 0x742d35Cc6634C0532925a3b844Bc9e7595e0bFa8 has a balance of 1,250.50 ANT tokens. The account nonce is 47, indicating 47 previous transactions. Status: Active.

---

**👤 You:**
> "Invoke the 'transfer' method on contract 'TokenContract' with args {"to": "0x123...", "amount": 100}."

**🤖 AI Agent:**
> ✅ Contract invocation successful! The 'transfer' method on 'TokenContract' executed successfully. Transaction hash: 0xdef456..., status: SUCCESS. Gas used: 45230. The transfer of 100 tokens to 0x123... has been confirmed on-chain.


## Installation & Usage

To install and use the **AntChain** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/antchain](https://vinkius.com/mcp/antchain)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
