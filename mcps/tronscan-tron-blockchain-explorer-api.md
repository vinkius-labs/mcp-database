# Tronscan (TRON Blockchain Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tronscan-tron-blockchain-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the TRON blockchain — analyze accounts, track token balances, inspect smart contracts, and monitor network resources directly from any AI agent.

## Description
Connect to the **Tronscan API** to turn your AI agent into a powerful blockchain analyst. Access real-time data from the TRON network, from simple balance checks to deep smart contract event auditing.

### What you can do

- **Account Intelligence** — Fetch detailed account profiles, including balance analysis, transaction history, and resource usage (Energy/Bandwidth).
- **Token Tracking** — List all TRC10, TRC20, TRC721, and TRC1155 tokens held by any address with precise balance reporting.
- **Smart Contract Auditing** — Inspect contract details, verify source code status, and retrieve live event logs for any deployed contract.
- **Resource Management** — Monitor Stake 1.0 and Stake 2.0 resources, voting status, and approval lists for governance participation.
- **Network Overview** — List top accounts and contracts to identify network trends and high-activity entities.

### How it works

1. Subscribe to this server
2. Enter your Tronscan Pro API Key
3. Start querying the TRON blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug smart contract events and check account resources without leaving your IDE.
- **Crypto Analysts** — perform deep on-chain analysis and track whale movements through natural language.
- **TRON Enthusiasts** — manage your votes, check rewards, and monitor your portfolio status instantly.


## Available Tools
- **get_account_analysis**: Get account analysis (Balance, Transfers, Energy, Bandwidth, Transactions)
- **get_account_detail**: Get detailed information for a specific account
- **get_account_security**: Get account security data
- **get_account_tags**: Get account behavioral tags
- **get_account_token_asset_overview**: Get token asset overview for an account
- **get_acquisition_cost_stats**: Get resource costs statistics
- **get_auth_security**: Get authorization security data
- **get_block_stats**: Get block statistics
- **get_chain_parameters**: Get chain parameters
- **get_consumption_stats**: Get burn/staking income statistics
- **get_contract_analysis**: Get contract daily analysis
- **get_contract_detail**: Get contract detail
- **get_contract_energy_stats**: Get contract energy statistics
- **get_contract_events**: Returns a list of event information for the contract
- **get_contract_top_calls**: Get contract call statistics
- **get_daily_accounts**: Get new users (daily)
- **get_daily_transactions**: Get transaction trend
- **get_energy_stats**: Get energy consumption statistics
- **get_funds**: Get TRX Supply & Marketcap
- **get_homepage_bundle**: Get homepage data bundle
- **get_multisign_security**: Get multi-sign security data
- **get_net_stats**: Get bandwidth consumption statistics
- **get_nodemap**: Get node map
- **get_stablecoin_big_amount**: Get stablecoin large transactions
- **get_stablecoin_blacklist**: Get stablecoin blacklist transactions
- **get_stablecoin_distribution**: Get stablecoin holder distribution
- **get_stablecoin_total_supply**: Get stablecoin total circulation
- **get_token_security**: Get token security data
- **get_top10**: Get Top 10 Data
- **get_tps**: Get current TPS
- **get_transaction_detail**: Get transaction detail
- **get_transaction_security**: Get transaction security data
- **get_trc10_token**: Get TRC10 token details
- **get_trc20_token**: Get TRC20/721/1155 token details
- **get_turnover**: Get total protocol revenue
- **get_url_security**: Get URL security data
- **list_account_resources**: Get account resources (Stake 1.0)
- **list_account_resources_v2**: Get account resources (Stake 2.0)
- **list_account_tokens**: Get tokens held by an account with balance > 0
- **list_account_votes**: Get account votes
- **list_accounts**: Get a list of accounts
- **list_approvals**: Get approval list for an account
- **list_blocks**: Get block list or detail
- **list_contracts**: Get list of smart contracts
- **list_internal_transactions**: Get internal transactions
- **list_proposals**: Get proposals
- **list_tokens_overview**: Get token list overview
- **list_transactions**: Get transaction list
- **list_transfers**: Get TRX & TRC10 transfers
- **list_trc10_holders**: Get TRC10 token holders
- **list_trc1155_inventory**: Get TRC1155 token inventory (NFTs)
- **list_trc1155_transfers**: Get TRC1155 token transfers
- **list_trc20_holders**: Get TRC20/721/1155 token holders
- **list_trc20_transfers**: Get TRC20 & TRC721 token transfers
- **list_trc721_inventory**: Get TRC721 token inventory (NFTs)
- **list_voted**: Get voted list for an account
- **list_witnesses**: Get witness list
- **search_v2**: Search Tronscan (v2)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tronscan (TRON Blockchain Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the detailed balance and analysis for address TXYZ..."

**🤖 AI Agent:**
> I've retrieved the analysis for address TXYZ... The account currently holds 1,500 TRX with an estimated total asset value of $180. Energy is at 95% capacity and Bandwidth is fully available.

---

**👤 You:**
> "List the top verified smart contracts on TRON sorted by transaction count."

**🤖 AI Agent:**
> Fetching the top verified contracts... The most active contract is currently 'USDT Token' (TR7NH...) with over 2 million transactions, followed by 'JustLend' and 'SunSwap'.

---

**👤 You:**
> "What are the recent events for the contract address TR7NH...?"

**🤖 AI Agent:**
> I've found the latest events for the USDT contract. Recent activities include multiple 'Transfer' events and 'Approval' updates. Would you like me to decode the parameters for the last five transfers?


## ❓ FAQ

**Q: Can I check the energy and bandwidth resources of a TRON account?**
Yes! You can use the `list_account_resources_v2` tool to get detailed information about Stake 2.0 resources, including available energy and bandwidth for any address.

**Q: How do I see all the TRC20 tokens held by a specific address?**
Use the `list_account_tokens` tool with the target address. You can filter by `show: 1` to specifically list TRC20 tokens and their current balances.

**Q: Is it possible to monitor live events from a smart contract?**
Yes. The `get_contract_events` tool allows you to retrieve a list of event information for a specific contract address, helping you track interactions and state changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tronscan-tron-blockchain-explorer-api](https://vinkius.com/mcp/tronscan-tron-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tronscan (TRON Blockchain Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tronscan-tron-blockchain-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tronscan (TRON Blockchain Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tronscan-tron-blockchain-explorer-api": {
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
