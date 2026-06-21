# Uniconta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uniconta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate ERP workflows via Uniconta — retrieve debtors, query invoices, manage GL accounts, and list inventory directly from any AI agent.

## Description
Connect your **Uniconta ERP** to any AI agent and take full enterprise control over global accounting ledgers, debtor/creditor relationships, and billing tracking securely natively via chat.

### What you can do

- **Client & Debtor Tracking** — List actively registered customers grabbing exact RowIDs or drill down into metadata isolating specific contact profiles via `get_debtor_details`
- **Invoicing & Billing Audits** — Fetch hundreds of active invoices tracking open debtor balances globally without manual filtering through ERP dashboards
- **General Ledger (GL) Supervision** — Query daily journals pulling transaction histories checking if the books map accurately
- **Inventory Verification** — Monitor product catalogs recovering item records, prices, and available stock configurations simultaneously

### How it works

1. Subscribe manually to this core server context
2. Introduce your personal Uniconta `Username`, `Password`, and targeting `Company ID`
3. Start mapping live invoice ledgers directly across Claude or your preferred integrated workspace

No digging into complicated Uniconta visual reports to pull a customer's address. Ask the AI and fetch exact company data natively instantly.

### Who is this for?

- **Financial Auditors** — request the AI to grab 'list_daily_journals' assessing transaction flows within 15 seconds without exporting massive Excel CSVs
- **Sales & Logistics** — swiftly verify stock numbers leveraging 'list_inventory_items' right from a chat window when building orders
- **Account Executives** — call down 'get_debtor_details' immediately before meetings checking exactly if their previous invoices remain unpaid


## Available Tools (8)
- **get_debtor_details**: Retrieves details for a specific debtor
- **list_gl_accounts**: Lists all General Ledger (GL) accounts in Uniconta
- **list_creditors**: Lists all creditors (vendors) registered in the ERP
- **list_debtors**: Lists all debtors (customers) registered in the ERP
- **list_employees**: Lists all employees registered in the Uniconta account
- **list_debtor_invoices**: Lists all debtor invoices issued by the company
- **list_inventory_items**: Lists all inventory items in the product catalog
- **list_daily_journals**: Lists all General Ledger daily journals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uniconta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Please provide the exact unformatted list of debtors actively open on this company's Uniconta profile."

**🤖 AI Agent:**
> I've fetched 22 root debtors successfully. The top three are "Global Tech Solutions" (RowId: 100), "Beta Widgets" (RowId: 104), and "Alpha Retail" (RowId: 121). Shall I grab more specific properties of any?

---

**👤 You:**
> "Look up our daily general ledger journals using the API."

**🤖 AI Agent:**
> Daily journals have been gathered. You have 3 pending batches currently registered under the accounting period mapping 'Q3'. Do you want the AI to analyze specific sub-transactions?

---

**👤 You:**
> "Fetch the metadata and details of Debtor ID 993 running in Uniconta."

**🤖 AI Agent:**
> Details isolated for ID 993: Legal Name represents "Acme Wholesale UK". Address logged sits at 1st London Ave. Their credit limit stands currently at max $250,000 threshold.


## ❓ FAQ

**Q: Can it search through all GL accounts at once?**
Yes. Command the LLM to 'list_gl_accounts'. It connects directly to the ERP tables handling your General Ledger mappings and provides a comprehensive, raw listing natively within seconds.

**Q: How do I securely retrieve the data from a single specific Debtor when preparing for a client call?**
Have the agent execute 'get_debtor_details' by supplying their account code or RowID. It extracts all assigned contacts, limits, local address formats, and primary balance metrics directly into reading text.

**Q: Is it possible to inspect pending inventory items and pricing directly dynamically and easily?**
Yes, trigger 'list_inventory_items' via standard chat protocols. The bot will automatically retrieve available catalogs, yielding active identifiers and current pricing arrays inherently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniconta](https://vinkius.com/mcp/uniconta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Uniconta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uniconta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Uniconta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uniconta": {
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
