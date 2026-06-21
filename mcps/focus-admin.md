# Focus Admin MCP Server

Send CC-e, inutilize numbering, distribute DF-e and list fiscal documents via Focus NFe API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-admin)

## Overview
**Category:** erp-operations
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Focus Admin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-admin](https://vinkius.com/mcp/focus-admin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
