# BlockPi (Distributed RPC Network) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockpi-distributed-rpc-network)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access distributed blockchain RPC nodes via BlockPi — monitor RU balances, track consumption, and execute JSON-RPC calls across multiple networks.

## Description
Connect your **BlockPi** account to any AI agent to manage your distributed RPC infrastructure and interact with blockchain networks directly through natural language.

### What you can do

- **Resource Monitoring** — Check your Request Unit (RU) balance and wallet balance in USD across different networks like Ethereum or Polygon.
- **Usage Analytics** — Track RU consumption over 1, 3, or 7 days to optimize your dApp's performance and infrastructure costs.
- **Package Management** — Inspect active RU packages, including SKU details, remaining amounts, and precise expiration timestamps.
- **Multi-Chain RPC** — Execute generic JSON-RPC calls (like `eth_blockNumber`, `eth_call`, or `eth_getBalance`) on Ethereum, BSC, Polygon, Solana, and more.

### How it works

1. Subscribe to this server
2. Enter your BlockPi API Key
3. Start querying blockchain data and managing your node resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly check node health, balances, and execute RPC methods without leaving the terminal or code editor.
- **DevOps Engineers** — monitor infrastructure consumption and package expiration to ensure zero downtime for decentralized applications.
- **Data Analysts** — fetch raw blockchain data directly through natural language queries using standard RPC methods.


## Available Tools
- **rpc_call**: g., eth_blockNumber, eth_call, eth_getBalance) on the specified network.

Make a generic JSON-RPC call to a supported blockchain network
- **get_package_expiration**: Get details about active RU packages
- **get_ru_balance**: Get remaining Request Unit (RU) balance
- **get_ru_consumed**: Get RU consumption for a specific endpoint
- **get_wallet_balance**: Get remaining wallet balance in USD


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlockPi (Distributed RPC Network)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my current RU balance and wallet balance on Ethereum."

**🤖 AI Agent:**
> I've checked your BlockPi account for the Ethereum network. You have 1,250,000 RU remaining and a wallet balance of $45.20 USD.

---

**👤 You:**
> "Show me the RU consumption for the last 3 days on Polygon."

**🤖 AI Agent:**
> In the last 3 days on the Polygon network, your endpoints have consumed a total of 450,000 RU.

---

**👤 You:**
> "Get the latest block number on Arbitrum using an RPC call."

**🤖 AI Agent:**
> Executing `eth_blockNumber` on Arbitrum... The current block height is 184,209,112.


## ❓ FAQ

**Q: How can I check my remaining Request Unit (RU) credits?**
You can use the `get_ru_balance` tool. Simply specify the network (e.g., 'ethereum') to see the current RU balance associated with your account.

**Q: Can I execute standard Ethereum methods like getting the latest block number?**
Yes! Use the `rpc_call` tool. Provide the network (e.g., 'ethereum') and the method name 'eth_blockNumber' to get real-time data from the blockchain.

**Q: How do I monitor my API usage over the last week?**
Use the `get_ru_consumed` tool and set the 'days' parameter to '7'. This will return the total RU consumption for your endpoints over that period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockpi-distributed-rpc-network](https://vinkius.com/mcp/blockpi-distributed-rpc-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlockPi (Distributed RPC Network)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blockpi-distributed-rpc-network` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlockPi (Distributed RPC Network)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blockpi-distributed-rpc-network": {
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
