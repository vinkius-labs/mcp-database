# Facturama (SAT) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/facturama-sat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Automate CFDI Mexico (SAT) Tax Invoices via Facturama — emit formal invoices, retrieve catalogs, and extract tax data fully relying on your AI.

## Description
Connect your **Facturama / SAT Mexico** corporative tax backend to any LLM and natively automate all bureaucratic burdens surrounding digital fiscal receipts (CFDI 4.0).

### What you can do

- **Live Ledger Invoice** — Pull all your recently emitted or pending electronic invoices, checking official CFDI statuses tied into SAT.
- **Catalog Maintenance** — Retrieve detailed registered products directly, fully validated against official government usage codex.
- **Invoice Emitting** — Tell Claude to emit a real transaction legally charging a verified Mexican client containing correct RFC values.
- **File Scraping** — Re-download lost PDFs or massive XML nodes natively generated holding digital timestamps representing valid commerce.

### How it works

1. Append this tax-heavy integration logic
2. Add your traditional basic auth API configuration bound in Private base64 streams directly on credentials config
3. You are ready to process accounting loops using pure natural chatting formats

### Who is this for?

- **Regional Accounting Leads** — Saving heavy hours navigating UI platforms trying to un-freeze single PDF bills.
- **eCommerce Operators** — Needing programmatic agents to check invoice status continuously in the background.
- **LATAM Startup Developers** — Probing Mexican tax RFC APIs fast utilizing just an active console and Claude interactions.


## Available Tools
- **create_client**: Register a new B2B invoice receiver
- **delete_client**: Remove receiver context
- **get_tax_status**: Read internal SAT compliance tax state
- **list_catalog**: Scan standard SAT codes
- **list_taxes**: Read internal schema tax profiles
- **send_invoice_email**: Push invoice via local mailer
- **cancel_invoice**: Cancel an issued CFDI / Invoice
- **create_invoice**: Issue a formal digital tax invoice (CFDI)
- **get_client**: Get a specific client fiscal profile
- **get_invoice_file**: Extract an invoice graphic representation (Base64 file)
- **get_product**: Fetch targeted product SAT specifics
- **list_clients**: List registered clients with tax details (RFC)
- **list_invoices**: List issued CFDIs (Tax Invoices)
- **list_products**: List tax-mapped registered products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Facturama (SAT)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check for recently emitted Valid CFDI invoices."

**🤖 AI Agent:**
> Running deep listing... I found 3 officially signed XML Invoices. Folio 001 issued 3 days ago for 'TechCorp Latam' carrying valid SAT standing, and Folio 002 for 'Local Business'. Both marked successfully Issued.

---

**👤 You:**
> "Check the detailed fiscal specifications for our currently registered client ID: C0098."

**🤖 AI Agent:**
> Sourced. Client ID 'C0098' belongs to 'Agencia Global S.A.' bearing the authentic SAT RFC tag 'AGE120092B08'. Their primary designated CFDI usage rule is set to 'G03 (Comercial Expenses)'. Ready to write an invoice against it?

---

**👤 You:**
> "Prepare and issue a new invoice. Sell Product ID p-3200 to Receiver ID c-099 using '01' as payment mode."

**🤖 AI Agent:**
> Done natively! I sent the exact construct containing proper payloads into Facturama endpoint. Result is positive: Generated CFDI with UUID `9E032A9A-1D8...`. It has been stamped officially by the SAT.


## ❓ FAQ

**Q: Can I bulk cancel tax invoices directly on the Mexican IRS bypassing visual interfaces?**
Yes. Utilize the `cancel_invoice` target tool carefully giving it the unique CFDI ID alongside the formal SAT motive parameter representing your reasoning, and it actively invalidates the fiscal stamp instantly at source.

**Q: How securely does the Basic Authentication hold within Vurb handling the Mexican invoices?**
The variables act as deep protected MCP credentials. You input them once securely mapping directly to fields labeled with generic `sensitive: true`. They transform cleanly into masked Base64 encodings locally and disappear off visual UI radar guaranteeing no accidental token logging into public clouds.

**Q: Can I retrieve a raw representation like PDF base64 of an older CFDI directly via Claude text generation?**
Absolutely. Deploy `get_invoice_file` referencing the exact entity ID while choosing between XML or PDF format outputs, granting heavy duty tracking across any calendar timeline seamlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/facturama-sat](https://vinkius.com/mcp/facturama-sat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Facturama (SAT)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `facturama-sat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Facturama (SAT)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "facturama-sat": {
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
