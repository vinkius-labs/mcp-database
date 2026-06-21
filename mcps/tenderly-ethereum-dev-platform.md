# Tenderly (Ethereum Dev Platform) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tenderly-ethereum-dev-platform)
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


## ❓ FAQ

**Q: Can I simulate a transaction without spending real ETH or gas?**
Yes! Use the `simulate_transaction` tool. It runs the transaction against the latest state of the network in a virtual environment, providing full trace and results without any on-chain cost.

**Q: How do I create a private fork of Ethereum for testing?**
You can use the `create_virtual_testnet` tool. Provide a slug, display name, and the network ID you want to fork from (e.g., 1 for Mainnet) to spin up a private RPC endpoint.

**Q: Can I monitor specific smart contract events automatically?**
Absolutely. Use the `create_alert` tool with an `alert_config` object to monitor method calls, state changes, or emitted logs on any contract address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenderly-ethereum-dev-platform](https://vinkius.com/mcp/tenderly-ethereum-dev-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tenderly (Ethereum Dev Platform)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tenderly-ethereum-dev-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tenderly (Ethereum Dev Platform)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tenderly-ethereum-dev-platform": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
