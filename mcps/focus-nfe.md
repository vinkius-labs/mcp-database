# Focus NFe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-nfe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Emit, consult, cancel and download XML for NFS-e and NF-e via Focus NFe API.

## Description
Connect **Focus NFe** to any AI agent and automate your Brazilian fiscal documentation — issue service invoices (NFS-e) and product invoices (NF-e), check status, cancel documents, and download XMLs via natural conversation.

### What you can do
- **Emit NFS-e** — Issue Service Invoices instantly
- **Emit NF-e** — Issue Product Invoices with full item details
- **Consult Status** — Check if a document is authorized, cancelled, or processing
- **Cancel Documents** — Cancel issued invoices with a justification reason
- **Download XML** — Retrieve the authorized XML for accounting and storage

### How it works
1. Subscribe to this server
2. Enter your Focus NFe API Token and Base URL
3. Start managing invoices from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Accountants** — Automate bulk invoice emission and XML retrieval
- **SaaS Platforms** — Integrate fiscal capabilities into their systems
- **Small Businesses** — Manage invoices directly through chat


## Available Tools (5)
- **cancel_document**: Cancel an authorized invoice
- **consult_document**: Consult the status and details of an invoice
- **download_xml**: Download the authorized XML document
- **emit_nfe**: Emit a Product Invoice (NF-e)
- **emit_nfse**: Emit a Service Invoice (NFS-e)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus NFe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Emit a service invoice for R$500 for 'Consulting Services'."

**🤖 AI Agent:**
> Service Invoice emitted! Reference: SERV-001. Status: Authorized.

---

**👤 You:**
> "Cancel invoice REF-123 with reason 'Client requested cancellation'."

**🤖 AI Agent:**
> Invoice REF-123 cancelled successfully.

---

**👤 You:**
> "Get the XML for invoice REF-123."

**🤖 AI Agent:**
> XML downloaded successfully. Ready for accounting integration.


## ❓ FAQ

**Q: Does it support both NFS-e and NF-e?**
Yes! The tools allow emitting and managing both Service Invoices (nfse) and Product Invoices (nfe) seamlessly.

**Q: How do I get my API Token?**
Log in to the Focus NFe portal and navigate to the API section to generate your token.

**Q: Can I download the authorized XML?**
Yes, use the `download_xml` tool with the document reference to retrieve the full XML content.

**Q: Is it homologated for all Brazilian cities?**
Focus NFe covers thousands of cities for NFS-e emission. You can check their API documentation for the complete list of supported IBGE city codes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-nfe](https://vinkius.com/mcp/focus-nfe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus NFe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `focus-nfe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus NFe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-nfe": {
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
