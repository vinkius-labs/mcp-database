# Plaid Enterprise Banking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plaid-enterprise-banking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Ultimate Open Banking: balances, transactions, ML fraud logic, payroll, and asset verification.

## Description
Connect your natural language AI directly to the **Plaid Enterprise** API ecosystem. Unlock Wall-Street grade financial intelligence by turning any compatible agent into a professional underwriter, forensic accountant, and wealth advisor.

### What you can do

- **Core Treasury** — Read available balances, credit limits, and sync L2/L3 enriched itemized transactions (merchants/geolocation).
- **Predictive ML (Signal & Network)** — Evaluate the fraud return risk of ACH wires before they happen via the Plaid Signal AI network.
- **Wealth & Liabilities** — Pull real-time brokerage investment holdings, asset reports, and audit credit card APR and student loan balances.
- **Payroll & Employment** — Parse and extract raw data from W2 payroll stubs and auto-verify active global employers.
- **AML & Watchlist Screening** — Check the account holder against the Interpol list, OFAC sanctions, and Global PEP for identity compliance.
- **Routing & ACH Wiring** — Safely extract account and 9-digit routing numbers securely for banking transfers.

### How it works

1. Subscribe to this server
2. Enter your Plaid Client ID and Secret in the setup
3. Pass your specific `access_token` into the LLM prompts to analyze isolated ledgers instantly

### Security Notice
This MCP instance is strictly hardcoded to **Read-Only**. While it can inspect mass volumes of wealth and ML data, it cannot programmatically execute ACH debits, Wires, or Payments on your behalf, ensuring production-grade safety.


## Available Tools (10)
- **create_link_token**: Required to connect bank accounts.

Create a Plaid Link token for account connection
- **exchange_public_token**: Exchange a public token for an access token
- **get_accounts**: List connected bank accounts
- **get_balances**: Get real-time account balances
- **get_categories**: List transaction categories
- **get_identity**: Get account holder identity
- **get_institution**: Get bank institution details
- **get_item_info**: Get connected item status
- **get_transactions**: Get transaction history
- **search_institutions**: Returns matching institutions with supported products.

Search financial institutions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plaid Enterprise Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here is the access token for the client: `access-prod-1234`. Can you fetch their current credit card outstanding liabilities and highlight any accounts charging over 20% APR?"

**🤖 AI Agent:**
> Querying the Liability engine... The user has $4,200 total revolving debt. The 'Chase Sapphire' card holds $3,100 at 19.99% APR, which is fine. However, their 'Amex Platinum' currently carries $1,100 at a steep **24.5% APR**. We should advise a balance transfer.

---

**👤 You:**
> "Investigate access token `access-prod-101` and check the investment brokerage holdings for AAPL and TSLA."

**🤖 AI Agent:**
> Connecting to the brokerage via Plaid Wealth... I extracted 15 security holdings. The client holds 125 shares of Apple (AAPL) priced at $185/share, yielding $23,125 total value. For Tesla (TSLA), they hold a massive 400 share position yielding a valuation of $72,000. Do you want to see the capital gains on those?

---

**👤 You:**
> "Using transaction access_token `access-prod-99`, analyze all ML recurring transaction signals. What subscriptions are they paying for?"

**🤖 AI Agent:**
> Running the Recurring Transactions Model... Plaid successfully detected 5 active passive flows on the main checking account: Netflix ($15.99), Spotify ($10.99), Equinox Gym ($205.00), AWS Cloud ($89.00), and an obscure app called 'AnyDo' ($4.99). Would you like to check the fraud signal prediction for these?


## ❓ FAQ

**Q: Is this safe to run against production Plaid accounts? Will the AI transfer money?**
Yes, it is entirely safe. We deliberately designed the 20 tools purely for deep inspection (fetching assets, checking IDs, balancing ledgers). Endpoints capable of moving capital (like `/transfer/create`) were excluded. The worst the AI can do is give you a highly detailed dashboard of your expenses.

**Q: How does the agent analyze different bank accounts when I talk to it?**
You hold the master Server keys (Client ID and Secret). When you ask the agent a question, you just paste or mention the unique `access_token` representing that customer's bank connection, and the AI automatically uses it under the hood.

**Q: Can it cross check watchlists (AML) and biometrics?**
Yes. Tools like `get_watchlist_screening` and `get_identity_verification` hook directly into Plaid Identity, matching end-users to PEP (Politically Exposed Persons), OFAC, and global government watchlists instantaneously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plaid-enterprise-banking](https://vinkius.com/mcp/plaid-enterprise-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plaid Enterprise Banking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plaid-enterprise-banking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plaid Enterprise Banking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plaid-enterprise-banking": {
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
