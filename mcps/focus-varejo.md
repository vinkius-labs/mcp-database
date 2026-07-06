# Focus Varejo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-varejo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Emit NFC-e, NFCom, manifest documents and manage retail invoices via Focus NFe API.

## Description
Connect **Focus Varejo** to any AI agent and manage your retail and telecom fiscal documentation — issue NFC-e for retail sales, NFCom for telecom services, manifest NF-e and CT-e as recipient, and list received NFS-e through natural conversation.

### What you can do
- **Emit NFC-e** — Issue Consumer Invoices for retail point-of-sale transactions
- **Emit NFCom** — Issue Communication/Telecom Service Invoices
- **Manifest NF-e** — Acknowledge or confirm invoices issued against your CNPJ
- **Manifest CT-e** — Acknowledge transport documents as recipient
- **Consult Status** — Check authorization and status of NFC-e and NFCom
- **List Received NFS-e** — View all service invoices received by your company

### How it works
1. Subscribe to this server
2. Enter your Focus NFe API Token and Base URL
3. Start managing retail documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Retail Stores** — Issue NFC-e for in-store sales without POS panel access
- **Telecom Companies** — Manage NFCom for communication services efficiently
- **Purchasing Departments** — Manifest NF-e and CT-e to confirm receipt of goods


## Available Tools (8)
- **manifest_cte**: Manifest CT-e as recipient
- **cancel_nfce**: Cancel NFC-e
- **consult_nfce**: Consult NFC-e status
- **consult_nfcom**: Consult NFCom status
- **emit_nfce**: Emit NFC-e for retail sales
- **emit_nfcom**: Emit NFCom for Telecom services
- **list_received_nfse**: List NFS-e received by the company
- **manifest_nfe**: Manifest NF-e as recipient (Ciência, Confirmação, etc)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus Varejo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Emit an NFC-e for a sale of R$89.90."

**🤖 AI Agent:**
> NFC-e emitted! Reference: NFC-001. Status: Authorized.

---

**👤 You:**
> "Manifest NF-e 3523010000000000000055001000001000 as confirmed."

**🤖 AI Agent:**
> Manifestation sent successfully. Event: Confirmation (210760).

---

**👤 You:**
> "List all service invoices received by CNPJ 12.345.678/0001-00."

**🤖 AI Agent:**
> Found 12 received NFS-e. Latest: Service from XYZ Company, R$500.00.


## ❓ FAQ

**Q: What is NFCom?**
NFCom (Nota Fiscal de Comunicação) is used for telecommunication services like internet, phone, and TV subscriptions.

**Q: Why should I manifest NF-e?**
Manifestation confirms that your company acknowledges receiving the goods. Events include Ciência da Operação (210750), Confirmação (210760), and others.

**Q: Can I list all NFS-e received by my company?**
Yes, use the `list_received_nfse` tool to see all service invoices where your company is the taker (tomador).

**Q: Can I emit an NFC-e offline?**
Yes, NFC-e allows issuance in offline contingency. Your AI agent can prepare and log the NFC-e locally until the connection is restored, then it will sync via the API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-varejo](https://vinkius.com/mcp/focus-varejo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus Varejo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `focus-varejo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus Varejo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-varejo": {
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
