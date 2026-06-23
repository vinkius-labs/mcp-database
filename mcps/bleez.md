# Bleez MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bleez)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Power your Brazilian e-commerce with a platform that integrates payments, inventory, and logistics for the local market.

## Description
Connect your **Bleez** account to any AI agent and take full control of your French accounting workflows and digital document management through natural conversation.

### What you can do

- **Ledger Orchestration** — List and manage accounting journal entries programmatically, retrieving detailed historical ledger data in real-time
- **Invoice Lifecycle Management** — Create and track sales and purchase invoices programmatically to maintain a perfectly coordinated billing pipeline
- **Document Ingestion** — Programmatically upload digital documents (PDF/Images) to the 'Factures à traiter' module for high-fidelity automated processing
- **Contact Discovery** — Access complete directories of customer and supplier profiles to coordinate your organizational relationship ecosystem
- **Folder Visibility** — Retrieve organization-level metadata and folder settings directly through your agent for instant financial reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Encrypted Folder Key** (Clé du dossier encryptée) from your Bleez dashboard (Administration > Dossier > Paramétrages)
3. Start managing your French accounting from Claude, Cursor, or any MCP client

No more manual entry into accounting tables or digging through paper files. Your AI acts as your dedicated French accountant and document coordinator.

### Who is this for?

- **Business Owners in France** — instantly retrieve invoice summaries and upload documents using natural language commands
- **Accountants** — monitor ledger entries and manage client directories without leaving your creative workspace
- **Developers** — integrate high-speed French accounting data into custom business workflows through simple AI queries


## Available Tools (8)
- **create_accounting_entry**: Provide date, label, and account lines.

Create a new accounting entry
- **create_invoice**: Provide contact ID and amount.

Create a new invoice
- **get_account_info**: Get current account settings
- **list_accounting_entries**: List all accounting journal entries
- **list_customers**: List all customers
- **list_invoices**: List all invoices
- **list_suppliers**: List all suppliers
- **upload_document**: Upload a digital document for processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bleez** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in my Bleez folder."

**🤖 AI Agent:**
> I've retrieved your client directory. You currently have 50 active customers, including 'Vinkius SARL' and 'Global Tech'. Would you like the detailed metadata for a specific contact?

---

**👤 You:**
> "Upload the file 'invoice_123.pdf' to Bleez for processing."

**🤖 AI Agent:**
> Document uploaded! I've successfully deposited 'invoice_123.pdf' into your 'Factures à traiter' module. Bleez is now processing the content for your ledger. Need help checking the status?

---

**👤 You:**
> "Show the last 5 accounting entries recorded this month."

**🤖 AI Agent:**
> Accessing ledger... I found 5 recent entries including a payment for 'Electricity' and 4 sales records. The total volume is within high-fidelity norms for April. Shall I retrieve the detailed account lines?


## ❓ FAQ

**Q: How do I find my Bleez Encrypted Folder Key?**
Log in to your Bleez account, navigate to **Administration** > **Dossier** > **Paramétrages**, and copy the **Clé du dossier encryptée**.

**Q: Can I upload invoices for processing via AI?**
Yes! The `upload_document` tool allows you to deposit PDF or image files directly into the Bleez automated processing queue programmatically.

**Q: Does it support French journal entries?**
Absolutely. The `list_accounting_entries` and `create_accounting_entry` tools are designed for standard French accounting ledger orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bleez](https://vinkius.com/mcp/bleez)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bleez** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bleez` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bleez** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bleez": {
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
