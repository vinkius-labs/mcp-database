# Conflux MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conflux)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Query Conflux Network (Core & eSpace) data — check balances, inspect blocks, and track transactions directly from your AI agent.

## Description
Connect to the **Conflux Network** and interact with both Core Space and eSpace through natural language. This server provides a comprehensive suite of tools to audit accounts, monitor network status, and analyze blockchain data.

### What you can do

- **Network Status** — Retrieve real-time node status, client versions, and the best block hashes from the Tree-Graph ledger.
- **Account Auditing** — Fetch CFX balances, nonces, and full account state summaries for any address on Core Space or eSpace.
- **Block & Epoch Analysis** — Inspect detailed block data by hash or epoch number, including full transaction objects.
- **Sponsorship Insights** — Query gas and storage sponsorship details for smart contracts on Core Space.
- **Transaction Tracking** — Retrieve transaction receipts and execution logs to debug or monitor on-chain activity.
- **Gas Estimation** — Calculate gas and collateral requirements for transactions before sending them to the network.

### How it works

1. Subscribe to this server
2. Provide your Conflux Core and eSpace RPC URLs
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug smart contracts and check account states directly from your IDE without switching to a block explorer.
- **Data Analysts** — extract epoch data and transaction logs for off-chain analysis using simple prompts.
- **Crypto Power Users** — monitor balances and sponsorship levels across multiple accounts in a unified conversation.


## Available Tools (25)
- **cfx_get_account**: Get summary of a Core Space account state
- **cfx_get_balance**: Get CFX balance of an address on Core Space
- **cfx_get_best_block_hash**: Get hash of the block with the highest weight
- **cfx_get_block_by_epoch_number**: Get Core Space block details by epoch number
- **cfx_get_block_by_hash**: Get Core Space block details by hash
- **cfx_get_blocks_by_epoch**: Get all block hashes in a specific Core Space epoch
- **cfx_call**: Execute a read-only contract call locally on Core Space
- **cfx_client_version**: Get Conflux Core client version
- **cfx_estimate_gas_and_collateral**: Estimate gas and storage collateral for a Core Space transaction
- **cfx_get_logs**: Get Core Space logs matching a filter
- **cfx_get_next_nonce**: Get next available nonce for a Core Space account
- **cfx_send_raw_transaction**: Send a pre-signed raw transaction to Core Space
- **cfx_send_transaction**: Requires the node to manage the sender account.

Send an unsigned transaction to the Core Space network
- **cfx_get_sponsor_info**: Get sponsorship details for a Core Space contract
- **cfx_get_status**: Get current state of the Conflux Core node
- **cfx_get_transaction_by_hash**: Get Core Space transaction details by hash
- **cfx_get_transaction_receipt**: Get Core Space transaction receipt
- **eth_get_balance**: Get balance of an address on eSpace
- **eth_get_block_by_number**: Get eSpace block details by number
- **eth_call**: Execute a read-only contract call locally on eSpace
- **eth_estimate_gas**: Estimate gas for an eSpace transaction
- **eth_get_logs**: Get eSpace logs matching a filter
- **eth_send_raw_transaction**: Send a pre-signed raw transaction to eSpace
- **eth_get_transaction_count**: Get transaction count (nonce) for an eSpace address
- **eth_get_transaction_receipt**: Get eSpace transaction receipt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conflux** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status and client version of the Conflux node?"

**🤖 AI Agent:**
> I've checked the node. The current epoch is 124,502,312 and the client version is 'conflux-rust/v2.3.0'. The network is currently stable and synchronized.

---

**👤 You:**
> "Check the balance and account state for address cfx:aak2rra2njvd77ezwjvx74749399393939393939."

**🤖 AI Agent:**
> The account has a balance of 1,250.45 CFX. The next available nonce is 42, and the account is currently active in the staking system.

---

**👤 You:**
> "Get the details of the block with hash 0x8e5f... and include full transactions."

**🤖 AI Agent:**
> I've retrieved block 0x8e5f... It contains 12 transactions. Notable transactions include a contract call to the 'Sponsor' system and several CFX transfers. Would you like to inspect a specific transaction receipt?


## ❓ FAQ

**Q: How can I check the CFX balance of a specific Core Space address?**
Use the `cfx_get_balance` tool by providing the Conflux address. You can also optionally specify an epoch (like 'latest_state') to get the balance at a specific point in time.

**Q: Can I see if a smart contract has gas or storage sponsorship?**
Yes! The `cfx_get_sponsor_info` tool returns the sponsorship details for any target contract address, showing who is covering the costs for users interacting with it.

**Q: How do I get the latest state of the Conflux Core network?**
Run the `cfx_get_status` tool. It provides the current epoch number, block height, chain ID, and other essential metrics about the node's synchronization state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conflux](https://vinkius.com/mcp/conflux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conflux** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conflux` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conflux** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conflux": {
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
