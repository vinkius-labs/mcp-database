# sevDesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sevdesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Empower your AI with direct read and write access to sevDesk to autonomously manage invoices, CRM contacts, sales orders, vouchers, and accounting records.

## Description
Grant your conversational AI (like Claude or Cursor) the power of a dedicated German accounting clerk. The **sevDesk MCP** transforms your LLM into a sophisticated financial nexus capable of creating invoices, querying past-due credit notes, recording vouchers, and tracking your CRM endpoints dynamically. Stop wrestling with browser-based accounting dashboards and let your AI manage your bookkeeping automatically.

### What you can do

- **Client & Supplier CRM Mastery** — Read the entire client database via `list_contacts`, retrieve detailed metadata for specific IDs (`get_contact`), or seamlessly register brand new vendors via `create_contact`
- **Autonomous Invoicing & Orders** — Fetch paginated ledger lists using `list_invoices` or `list_orders`, and delve deep into line items, calculated taxes, and due statuses directly using `get_invoice` and `get_order`
- **Inventory & Service Architecture** — Monitor available billable components via `list_parts`, inspect standard pricing, and introduce novel catalog options autonomously via `create_part`
- **Accounting Governance** — Keep strict tabs on your chart of accounts with `list_accounting_types` while verifying associated business inlets securely using `list_bank_accounts`
- **Voucher & Credit Auditing** — Consolidate physical receipts through `list_vouchers` and trace structural adjustments flawlessly by scanning `list_credit_notes`

### How it works

1. Install this module directly into your MCP-compatible IDE or conversational context
2. Establish the secure connection effortlessly by injecting your 32-character hexadecimal `sevDesk API Token`
3. Engage your AI explicitly: "What's the net total on invoice #392911, and who is the attached client?"

### Who is this for?

- **Freelancers & Solopreneurs** — quickly ask your agent to draft new customer records and extract pending invoice tallies without leaving the editor
- **Financial Auditors** — instruct the AI to cross-reference registered parts and orders against generated credit notes natively
- **Agency Managers** — effortlessly check current bank configuration parameters and available accounting categories entirely via conversational prompts


## Available Tools (15)
- **create_contact**: Category 3 for customers, 4 for suppliers.

Creates a new contact (customer or supplier) in sevDesk
- **get_invoice**: Retrieves details for a specific invoice, including line items and tax
- **list_credit_notes**: Lists all credit notes
- **get_credit_note**: Retrieves details for a specific credit note
- **list_orders**: Lists all sales orders
- **get_order**: Retrieves details for a specific order
- **list_vouchers**: Lists all vouchers (incoming/outgoing receipts)
- **list_parts**: Lists all parts (products and services) in the catalog
- **get_part**: Retrieves details for a specific part
- **create_part**: Creates a new part or service in the catalog
- **list_accounting_types**: Lists all accounting types (Chart of Accounts)
- **list_bank_accounts**: Lists company bank accounts
- **list_contacts**: Lists all contacts (customers, suppliers) in sevDesk
- **get_contact**: Retrieves details for a specific contact
- **list_invoices**: Lists all invoices with embedded contact data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **sevDesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the details of invoice #18742 and summarize its line items alongside the associated contact name."

**🤖 AI Agent:**
> Invoking `get_invoice` using ID 18742 successfully queried the sevDesk API endpoint. The underlying contact reference resolves beautifully to the recognized entity "Stark Industries". Inspecting the associated line-item array reveals two dominant artifacts currently billed: Software Maintenance Support (15 units representing hourly increments at 120.00 each) and Cloud Expansion Licensing Cost (a flat 400.00 fee). The overall net calculation indicates 2200.00 EUR dynamically computed without outstanding adjustments. Do you wish to verify its status in `list_credit_notes` to rule out refunds?

---

**👤 You:**
> "List all currently existing bank accounts natively integrated using the core config."

**🤖 AI Agent:**
> Running the targeted diagnostic `list_bank_accounts` extracted exactly 2 live inlets formally structured under this tenant entity. Check account 001 maps to the primary 'Deutsche Bank GmbH' with an active balancing status indicating ready-reckoner liquidity. Setup inlet 002 flags explicitly as the secondary 'Commerzbank Corporate Node' reserve. Both objects exhibit identical local currency encodings (EUR).


## ❓ FAQ

**Q: Are API-created contacts exactly the same as UI-created ones?**
Yes contextually. When you execute the `create_contact` function natively alongside `category` parameters (`3` stands for customer, `4` for typical suppliers), sevDesk anchors these entries officially inside the identical primary table. Be clear about whether it's an email-lead versus a firm.

**Q: Wait, does my generated API Token expire if left unused?**
No. The verified 32-character hexadecimal key token possesses an infinite lifeline inherently tied directly, securely, and stubbornly to your primary login account. It decays or dies primarily upon deliberate manual revocation (regeneration) directly executed by you inside your dashboard user settings.

**Q: Can I fetch detailed line items from a single invoice ID using this agent?**
Absolutely. Querying `list_invoices` outputs high-level paginated arrays, but invoking the precision extractor `get_invoice` fed deliberately with a target identifier ID unveils the core metadata array detailing isolated tax mappings, due-date boundaries, and intricate line items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sevdesk](https://vinkius.com/mcp/sevdesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **sevDesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sevdesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **sevDesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sevdesk": {
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
