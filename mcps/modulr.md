# Modulr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modulr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Empowers algorithmic control over European Payment volumes. Execute massive HMAC-secured payment schedules, create internal ledgers natively.

## Description
The **Modulr MCP Server** wraps incredibly defensive digital signatures (HMAC SHA-256) autonomously underneath a native Language Model Chat interface. Meaning, your AI has programmatic limits to fire secure European and British payment rails on command natively.

### Core Functionality

- **Create Modulr Customers/Accounts** — Manage deeply nested multi-layered B2B structures. Automatically provision Sort-Code ledgers via `modulr_create_account`.
- **Payment Initiation** — Run automated payroll or contractor compensation logic utilizing direct clearing paths mapping via `modulr_create_payment`.
- **Algorithmic Tracing** — Check real-time payment states checking failures or settlements organically utilizing `modulr_list_payments`.

### How it works

1. From your Modulr Finance administrative interface, spawn your API Key Profile and the underlying API Secret Hash.
2. Vinkius natively utilizes the `MODULR_API_SECRET` not as a password, but natively applying a Cryptographic Hash generating Nonces and Date Timestamps implicitly on every Chat-driven Tool call to authenticate accurately with European servers.

### Use Cases

- **Lending Startups** — Direct integration validating funds exactly when needed.
- **Payment Reconciliations** — Have the Agent review your physical transactional ledger.


## Available Tools (7)
- **modulr_create_account**: g. GBP or EUR).

Instantiate a UK/EU Account under a specific Customer
- **modulr_create_beneficiary**: , or IBAN.

Map an external Recipient
- **modulr_create_payment**: Trigger an outgoing Faster Payment or SEPA payout
- **modulr_get_accounts**: List all live Accounts and mapped liquidity
- **modulr_get_customers**: List underlying legal customers/entities inside Modulr
- **modulr_get_transactions**: Audit transaction histories on a specific Account
- **modulr_list_payments**: Check the status of massive payment arrays


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modulr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check our main UK sub-account. View the history array mapped onto it to find pending activity."

**🤖 AI Agent:**
> Ledger analysis received intact from the Modulr engine. Validating Account details, your latest block exposes 2 internal pending transfers reflecting cleared Faster Payments routes to standard banks without error.

---

**👤 You:**
> "Initialize a payment stream. Register a Beneficiary named 'DevTeam' pointing to target Sort Code 123456 Acct 98765432. Send £5,000 from Account 'A110' natively."

**🤖 AI Agent:**
> Payment routed through Faster Payment nodes seamlessly via API keys validating successful HMAC verification! Target beneficiary successfully populated inside your dashboard bounds resulting natively into £5000 liquid push.

---

**👤 You:**
> "Scan our Modulr operational Customers and list the active instances returning metadata boundaries."

**🤖 AI Agent:**
> Operation verified. Modulr confirmed your primary Customer instance identified as: C11XXXX. Available limits are active.


## ❓ FAQ

**Q: Modulr requires complex timestamped HMAC API Signatures, how does the prompt handle that?**
We handle that completely in the background Engine! The Vinkius runtime grabs your static API Secret from configurations once. Then, every time the Language Model triggers a payment, our Node.js runtime creates random cryptographic hex Nonces, aligns current UTC Date limits, hashes the combination uniquely via SHA-256 and packs it into the underlying header dynamically natively.

**Q: Can the Agent generate new SEPA/UK Accounts?**
Yes, using `modulr_create_account`, you can spawn multiple isolated UK GBP ledgers natively linked to customers.

**Q: Are cross-border Faster Payments supported natively?**
Absolutely. You can inject external sorts codes inside the `modulr_create_payment` orchestrations delivering funds transparently via clearing houses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modulr](https://vinkius.com/mcp/modulr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Modulr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `modulr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Modulr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "modulr": {
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
