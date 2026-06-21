# Tenderly (Ethereum Dev Platform) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tenderly-ethereum-dev-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tenderly-ethereum-dev-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tenderly-ethereum-dev-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Simulate Ethereum transactions, create Virtual TestNets, and monitor on-chain events directly from your AI agent.

## Description
Connect your **Tenderly** account to any AI agent to streamline your Ethereum development workflow. This MCP server allows you to debug, simulate, and monitor smart contracts through natural language.

### What you can do

- **Transaction Simulation** — Simulate single transactions or complex bundles on any supported network without committing real assets or spending gas.
- **Virtual TestNets** — Create and manage private mainnet replicas (Virtual TestNets) to test your dApps in a production-like environment with custom configurations.
- **On-Chain Monitoring** — Set up sophisticated alerts for method calls, state changes, or value transfers to stay informed about blockchain activity in real-time.
- **Bundle Execution** — Test sequences of transactions to see how they interact, perfect for debugging complex DeFi protocols or multi-step workflows.

### How it works

1. Subscribe to this server
2. Provide your Tenderly Access Key, Account Slug, and Project Slug
3. Start simulating transactions and managing testnets from Claude, Cursor, or any MCP client

### Who is this for?

- **Smart Contract Engineers** — debug transactions and verify contract behavior before deployment.
- **DeFi Researchers** — simulate complex multi-step transactions to analyze protocol interactions.
- **Web3 DevOps** — monitor production contracts and manage private testing environments seamlessly.


## Available Tools
- **create_alert**: Expression types include method_call, state_change, tx_value, emitted_log, eth_balance.

Create an alert on Tenderly
- **create_virtual_testnet**: Create a Virtual TestNet on Tenderly
- **simulate_bundle**: Simulate a bundle of transactions on Tenderly
- **simulate_transaction**: Simulate a transaction on Tenderly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tenderly (Ethereum Dev Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate a transaction on Ethereum Mainnet from 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045 to 0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D with data 0x095ea7b3..."

**🤖 AI Agent:**
> I've simulated the transaction. The simulation was successful, consuming 45,000 gas. It would result in an ERC20 Approval event for the Uniswap V2 Router. Would you like to see the full state changes?

---

**👤 You:**
> "Create a Virtual TestNet named 'Staging-Fork' forked from Mainnet at the latest block."

**🤖 AI Agent:**
> Virtual TestNet 'Staging-Fork' has been created successfully. You can now access it via the generated RPC URL. The Chain ID is set to your specified virtual ID.

---

**👤 You:**
> "Set up an alert to notify me whenever the 'transfer' method is called on contract 0x123..."

**🤖 AI Agent:**
> I've created the alert for contract 0x123... monitoring the 'transfer' method. You will receive notifications based on your Tenderly project settings whenever this event is detected on-chain.


## Installation & Usage

To install and use the **Tenderly (Ethereum Dev Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenderly-ethereum-dev-platform](https://vinkius.com/mcp/tenderly-ethereum-dev-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
