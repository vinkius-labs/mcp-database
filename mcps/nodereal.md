# Nodereal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nodereal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

High-performance blockchain infrastructure for Aptos and EVM networks — query accounts, blocks, and simulate transactions.

## Description
Connect to **NodeReal**, the ultimate high-performance blockchain infrastructure provider. This MCP server allows any AI agent to interact directly with Aptos and EVM-compatible networks through reliable RPC endpoints.

### What you can do

- **Aptos Ecosystem** — Retrieve account details, resources, and Move modules. Inspect ledger info, blocks, and transaction history using specialized Aptos tools.
- **EVM Compatibility** — Access standard JSON-RPC methods for Ethereum-compatible chains, including block numbers, chain IDs, and account balances.
- **Transaction Simulation** — Use `aptos_simulate_transaction` to estimate gas and validate execution logic before committing to the network.
- **Deep Data Inspection** — Fetch detailed transaction receipts and filter logs via `eth_get_logs` for complex on-chain analysis.
- **Real-time Queries** — Get the most recent block data and network state instantly.

### How it works

1. Subscribe to this server
2. Enter your NodeReal API Endpoint URL
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug smart contracts and check account states directly from your IDE.
- **Data Analysts** — extract on-chain logs and transaction metadata for research and reporting.
- **DevOps Engineers** — monitor network height and chain connectivity through simple natural language commands.


## Available Tools (24)
- **aptos_get_account_modules**: Get all Move modules for a specific Aptos account
- **aptos_get_account_resources**: Get all resources for a specific Aptos account
- **aptos_get_account**: Get high-level information about an Aptos account
- **aptos_get_blocks_by_height**: Get Aptos blocks by height
- **aptos_get_ledger_info**: Get the current Aptos ledger information
- **aptos_get_transaction_by_hash**: Get an Aptos transaction by its hash
- **aptos_get_transactions**: Get a list of Aptos transactions
- **aptos_simulate_transaction**: Simulate an Aptos transaction submission
- **debug_trace_transaction**: Trace a transaction (EVM)
- **eth_block_number**: Get the current block number (EVM)
- **eth_call**: Execute a new message call immediately without creating a transaction (EVM)
- **eth_chain_id**: Get the chain ID (EVM)
- **eth_estimate_gas**: Generates and returns an estimate of how much gas is necessary to allow the transaction to complete (EVM)
- **eth_get_balance**: Get the balance of an address (EVM)
- **eth_get_block_by_number**: Get a block by its number (EVM)
- **eth_get_logs**: Get logs matching a given filter object (EVM)
- **eth_get_transaction_receipt**: Get the receipt of a transaction (EVM)
- **eth_send_raw_transaction**: Creates new message call transaction or a contract creation for signed transactions (EVM)
- **nr_get_asset_transfers**: Get asset transfers for an address (NodeReal Enhanced)
- **nr_get_nft_holders**: Get holders of an NFT collection (NodeReal Enhanced)
- **nr_get_nft_inventory**: Get NFT inventory for an address (NodeReal Enhanced)
- **nr_get_token_balance_20**: Get ERC20 token balance (NodeReal Enhanced)
- **nr_get_token_holders**: Get list of token holders (NodeReal Enhanced)
- **nr_get_transaction_receipts_by_block_number**: Get all receipts in a block (NodeReal Enhanced)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nodereal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current block number for the configured EVM network."

**🤖 AI Agent:**
> I've queried the network using `eth_block_number`. The current block height is 18,452,103.

---

**👤 You:**
> "Retrieve account information for Aptos address 0x1."

**🤖 AI Agent:**
> Using `aptos_get_account`, I found that address 0x1 has a sequence number of 5234 and an authentication key ending in ...a3f2.

---

**👤 You:**
> "Check the ETH balance for address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e."

**🤖 AI Agent:**
> I've executed `eth_get_balance`. The balance for that address is 1.25 ETH (represented as 1250000000000000000 wei).


## ❓ FAQ

**Q: Can I check the resources associated with an Aptos account?**
Yes, you can use the `aptos_get_account_resources` tool by providing the account address to see all Move resources stored on that account.

**Q: How do I retrieve logs for a specific smart contract on an EVM chain?**
Use the `eth_get_logs` tool. You will need to provide a JSON filter object containing parameters like the contract address and block range.

**Q: Is it possible to test an Aptos transaction without actually sending it?**
Absolutely. The `aptos_simulate_transaction` tool allows you to submit a transaction payload to see if it would succeed and how much gas it would consume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nodereal](https://vinkius.com/mcp/nodereal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nodereal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nodereal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nodereal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nodereal": {
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
