# Focus Admin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-admin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Send CC-e, inutilize numbering, distribute DF-e and list fiscal documents via Focus NFe API.

## Description
Connect **Focus Admin** to any AI agent and access advanced fiscal management tools — send Correction Letters (CC-e), inutilize NF-e numbering, distribute DF-e documents, download XMLs and DANFEs, and list all invoices by period through natural conversation.

### What you can do
- **Send CC-e** — Issue Correction Letters for authorized NF-e with minor errors
- **Cancel CC-e** — Cancel previously sent Correction Letters
- **Inutilize Numbering** — Mark damaged or lost NF-e numbering ranges as unused
- **Download XML & DANFE** — Retrieve authorized NF-e XML documents and DANFE PDFs
- **Distribute DF-e** — Query available DF-e documents for your CNPJ by NSU
- **List by Period** — Retrieve all NF-e or NFS-e issued or received within a date range
- **Download Event XML** — Get XML for specific NF-e events (manifestations, CC-e, etc.)

### How it works
1. Subscribe to this server
2. Enter your Focus NFe API Token and Base URL
3. Start managing advanced fiscal operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Fiscal Analysts** — Handle CC-e and inutilization without accessing the fiscal panel
- **Accounting Teams** — Download XML/DANFE in bulk and list documents by period
- **Compliance Officers** — Distribute DF-e and verify all received invoices


## Available Tools
- **send_cc_e**: Send a Correction Letter (CC-e) for NF-e
- **cancel_cc_e**: Cancel a previously sent CC-e
- **distribute_dfe**: Distribute DF-e documents (consult NSU)
- **download_nfe_danfe**: Download NF-e DANFE PDF
- **download_nfe_xml**: Download NF-e XML document
- **download_event_xml**: Download XML for a specific NF-e event
- **inutilize_numbering**: Inutilize a range of NF-e numbering
- **list_nfse_emitted**: List NFS-e emitted by the company
- **list_nfse_received**: List NFS-e received (tomadas) by the company
- **list_nfe_by_period**: List NF-e documents by period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus Admin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a CC-e for NF-e REF-001 correcting the buyer's phone number."

**🤖 AI Agent:**
> CC-e sent successfully! Protocol: 123456789.

---

**👤 You:**
> "Inutilize NF-e numbering from 1000 to 1050 for series 1, model 55, year 2026."

**🤖 AI Agent:**
> Numbering range 1000-1050 successfully inutilized for series 1.

---

**👤 You:**
> "List all NF-e issued by CNPJ 12.345.678/0001-00 from 2026-03-01 to 2026-03-31."

**🤖 AI Agent:**
> Found 47 NF-e documents in the specified period.


## ❓ FAQ

**Q: What is a CC-e (Carta de Correção)?**
CC-e is a Correction Letter used to fix minor errors in an authorized NF-e, such as typos in the buyer's address or product descriptions. It cannot be used to change values, quantities, or tax rates.

**Q: When should I use Inutilização?**
Use Inutilização when a range of NF-e numbering has been damaged, lost, or will not be used. This tells the tax authority that those numbers are intentionally skipped.

**Q: What is DF-e Distribution?**
DF-e Distribution allows you to query all fiscal documents (NF-e, CT-e, etc.) issued against your CNPJ. Use it with the last NSU to retrieve only new documents.

**Q: Can I automate my accounting department with this?**
Yes! The 'List by Period' and 'Download XML & DANFE' tools allow your AI agent to fetch all invoices from a specific month, download the XMLs, and seamlessly integrate them into accounting workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-admin](https://vinkius.com/mcp/focus-admin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus Admin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `focus-admin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus Admin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-admin": {
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
