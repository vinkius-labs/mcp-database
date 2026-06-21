# Focus Varejo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/focus-varejo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/focus-varejo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/focus-varejo-mcp)
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


## Available Tools
- **cancel_nfce**: Cancel NFC-e
- **consult_nfce**: Consult NFC-e status
- **consult_nfcom**: Consult NFCom status
- **emit_nfce**: Emit NFC-e for retail sales
- **emit_nfcom**: Emit NFCom for Telecom services
- **list_received_nfse**: List NFS-e received by the company
- **manifest_cte**: Manifest CT-e as recipient
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


## Installation & Usage

To install and use the **Focus Varejo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/focus-varejo](https://vinkius.com/mcp/focus-varejo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
