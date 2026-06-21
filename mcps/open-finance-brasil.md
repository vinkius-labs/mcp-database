# Open Finance Brasil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-finance-brasil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect Open Finance Brasil to any AI agent via MCP.



## Available Tools
- **get_accounts**: Returns account type, agency, number, and available balance.

Get list of payment accounts and their balances
- **get_credit_card_bills**: Needs a Credit Card Account ID.

Get credit card bills for a specific card account
- **get_credit_cards**: Returns brand, limits (total, available, used).

Get credit card accounts and their limits
- **get_customer_data**: Returns basic identification info.

Get personal data of the customer (Name, CPF, Address)
- **get_financing**: Returns loans, vehicle financing, real estate.

Get financing and loan contracts
- **get_investments**: Returns treasury, funds, CDBs, etc.

Get investment portfolio
- **get_transactions**: Needs an Account ID from get_accounts.

Get transaction history for a specific account






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-finance-brasil](https://vinkius.com/mcp/open-finance-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Finance Brasil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-finance-brasil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Finance Brasil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-finance-brasil": {
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
