# GetBlock (Web3 RPC Provider) MCP Server

Access 50+ blockchain networks (Ethereum, Solana, Bitcoin) via RPC. Query balances, blocks, and transactions directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/getblock-web3-rpc-provider)

## Overview
**Category:** developer-tools
**Tools Count:** 26

## Description
Connect your **GetBlock** account to any AI agent and interact with dozens of blockchain protocols through natural conversation. GetBlock provides high-performance RPC node access for developers and crypto enthusiasts.

### What you can do

- **Multi-Chain Queries** — Fetch data from Ethereum, Solana, Bitcoin, and 50+ other supported networks using specialized tools.
- **Account & Balance Tracking** — Check native balances and token holdings across different chains (e.g., `eth_get_balance`, `sol_get_balance`).
- **Blockchain Inspection** — Retrieve block details, transaction receipts, and blockchain metadata (e.g., `eth_block_number`, `btc_get_blockchain_info`).
- **Advanced Debugging** — Access deep transaction traces and call simulations to analyze smart contract behavior (e.g., `debug_trace_transaction`).
- **Generic RPC Access** — Use the `rpc_call` tool to execute any JSON-RPC method supported by the GetBlock nodes.

### How it works

1. Subscribe to this server
2. Enter your GetBlock Access Token (API Key)
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug transactions and check contract states without leaving your code editor.
- **Crypto Analysts** — pull real-time on-chain data and block statistics for reporting and research.
- **DeFi Users** — monitor wallet balances and transaction statuses across multiple protocols via a single interface.


## Available Tools
- **btc_analyzepsbt**: Analyze and provide information about a PSBT
- **btc_createpsbt**: Create a transaction in the Partially Signed Bitcoin Transaction format
- **btc_getbestblockhash**: Get the hash of the best (tip) block
- **btc_getblockcount**: Get the number of blocks in the longest blockchain
- **btc_getblockchaininfo**: Get an object containing various state info regarding blockchain processing
- **btc_sendrawtransaction**: Submit raw transaction (serialized, hex-encoded) to local node and network
- **debug_trace_block_by_number**: Get traces for all transactions in a block
- **debug_trace_call**: Run an eth_call within the context of the given block execution
- **debug_trace_transaction**: Get all traces of a given transaction
- **eth_accounts**: Get a list of addresses owned by client
- **eth_block_number**: Get the number of the most recent block
- **eth_call**: Execute a new message call immediately without creating a transaction
- **eth_estimate_gas**: Estimate gas necessary to allow the transaction to complete
- **eth_get_balance**: Get the balance of an Ethereum account
- **eth_get_block_by_hash**: Get information about a block by hash
- **eth_get_block_by_number**: Get information about a block by block number
- **eth_get_code**: Get code at a given address
- **eth_get_transaction_by_hash**: Get information about a transaction by hash
- **eth_get_transaction_receipt**: Get the receipt of a transaction by hash
- **rpc_call**: Execute any generic JSON-RPC method via GetBlock
- **sol_get_account_info**: Get all information associated with the account of provided Pubkey
- **sol_get_balance**: Get the balance of the provided Pubkey
- **sol_get_latest_blockhash**: Get the latest blockhash from the ledger
- **sol_get_token_account_balance**: Get the token balance of an SPL Token account
- **sol_get_transaction**: Get transaction details for a confirmed transaction signature
- **sol_send_transaction**: Submit a signed transaction to the cluster for processing


## Installation & Usage

To install and use the **GetBlock (Web3 RPC Provider)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getblock-web3-rpc-provider](https://vinkius.com/mcp/getblock-web3-rpc-provider)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
