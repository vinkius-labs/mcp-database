# Focus Logística MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-logistica)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Emit CT-e, MDF-e, manage cargo manifests and transport documents via Focus NFe API.

## Description
Connect **Focus Logística** to any AI agent and manage your Brazilian cargo transport documentation — issue CT-e (Conhecimento de Transporte), MDF-e (Manifesto de Carga), close manifests, and download XMLs through natural conversation.

### What you can do
- **Emit CT-e** — Issue transport invoices for all modalities (road, air, rail, waterway)
- **Emit MDF-e** — Create cargo manifests grouping multiple CT-e documents
- **Consult Status** — Check authorization and current status of CT-e and MDF-e
- **Close Manifests** — Mark MDF-e as finished/encerrado after delivery
- **Cancel Documents** — Cancel CT-e with valid justification
- **Download XML** — Retrieve XML for accounting and legal compliance

### How it works
1. Subscribe to this server
2. Enter your Focus NFe API Token and Base URL
3. Start managing logistics documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Logistics Managers** — Issue CT-e and MDF-e without accessing the transport panel
- **Freight Companies** — Manage multiple transport documents and manifests efficiently
- **Accounting Firms** — Retrieve XML and verify status for client compliance


## Available Tools
- **close_mdfe**: Close/Finish a MDF-e
- **consult_cte**: Consult CT-e status
- **consult_mdfe**: Consult MDF-e status
- **download_xml**: Download XML for CT-e or MDF-e
- **emit_cte**: Emit a Conhecimento de Transporte (CT-e)
- **emit_mdfe**: Emit Manifesto de Carga (MDF-e)
- **cancel_cte**: Cancel a CT-e


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus Logística** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Emit a CT-e for a freight of R$1,200.00 from SP to RJ."

**🤖 AI Agent:**
> CT-e emitted successfully! Reference: CTE-001. Status: Authorized.

---

**👤 You:**
> "Close the MDF-e reference MDF-001."

**🤖 AI Agent:**
> MDF-e MDF-001 closed successfully.

---

**👤 You:**
> "Download the XML for CT-e reference CTE-001."

**🤖 AI Agent:**
> XML downloaded. Ready for accounting integration.


## ❓ FAQ

**Q: What transport modalities are supported for CT-e?**
CT-e supports all modalities: road (rodoviário), air (aéreo), rail (ferroviário), waterway (aquaviário), pipeline (dutoviário) and multimodal.

**Q: When should I close an MDF-e?**
You should close the MDF-e after the delivery is completed. Use the close_mdfe action to mark it as finished.

**Q: Can I cancel an authorized CT-e?**
Yes, as long as it hasn't been used for transport yet. Use cancel_cte with a valid justification reason.

**Q: What documents are required to generate an MDF-e?**
You need the related NFe (for own cargo) or CTe (for third-party cargo) references, as well as the vehicle's license plate and the driver's CPF.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-logistica](https://vinkius.com/mcp/focus-logistica)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus Logística** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `focus-logistica` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus Logística** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-logistica": {
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
