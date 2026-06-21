# Simple Fatoora MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simple-fatoora)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/simple-fatoora-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/simple-fatoora-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate ZATCA-compliant electronic invoices for Saudi Arabian businesses with automated tax calculations and QR code embedding.

## Description
Connect your **Simple Fatoora** account to any AI agent and take full control of your e-invoicing and business financial orchestration through natural conversation. Simple Fatoora provides a specialized platform for creating ZATCA-compliant invoices and managing small business accounting, and this integration allows you to retrieve invoice metadata, manage client databases, and track inventory directly from your chat interface.

### What you can do

- **Invoicing Orchestration** — Create simplified and VAT invoices programmatically to ensure your billing is always compliant and efficient.
- **Client Lifecycle Management** — List all managed clients and retrieve detailed profile metadata, including contact and tax info directly from the AI interface.
- **Inventory & Item Control** — Access and monitor your item database to keep your product and service catalog updated via natural language.
- **Financial Monitoring** — Retrieve and monitor invoice statuses to ensure your accounts receivable are always synchronized.
- **Operational Oversight** — Track account activity and manage inventory items using simple AI commands to streamline your business workflows.

### How it works

1. Subscribe to this server
2. Enter your Simple Fatoora API Key from your dashboard settings
3. Start managing your e-invoicing from Claude, Cursor, or any MCP-compatible client

No more manual ZATCA reporting or spreadsheet billing. Your AI acts as a dedicated accountant or finance operations manager.

### Who is this for?

- **Business Owners in KSA** — quickly generate ZATCA-compliant invoices and monitor client payments without switching apps.
- **Accountants & Finance Teams** — automate the retrieval of invoice metadata and monitor inventory levels via natural conversation.
- **Operations Managers** — streamline the management of client records and track item availability directly within the chat.


## Available Tools
- **create_client**: Create a new client
- **create_item**: Create a new item
- **create_simplified_invoice**: Pass items as a JSON string.

Create a Simplified Tax Invoice (B2C)
- **create_vat_invoice**: Pass items as a JSON string.

Create a VAT Tax Invoice (B2B)
- **delete_client**: Delete a client
- **get_client**: Get client details by ID
- **get_invoice**: Get invoice details by ID
- **list_clients**: List all clients
- **list_invoices**: List all invoices
- **list_items**: List all items/products
- **update_client**: Update an existing client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simple Fatoora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active invoices in Simple Fatoora."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 5 active records including 'INV-1001' (Paid) and 'INV-1002' (Draft). Would you like the full PDF data for any of them?

---

**👤 You:**
> "Create a simplified invoice for client 'John Miller' with a 'Consultation' item for 500 SAR."

**🤖 AI Agent:**
> Simplified invoice created! Client: John Miller, Item: Consultation, Total: 500 SAR. The invoice is ZATCA-compliant. Should I retrieve the QR code data for you?

---

**👤 You:**
> "Search for a client named 'Acme Corp' in my database."

**🤖 AI Agent:**
> Searching clients... I found one match for 'Acme Corp' (ID: 98765). They have a registered VAT number and 3 previous invoices. Would you like to see their contact history?


## Installation & Usage

To install and use the **Simple Fatoora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simple-fatoora](https://vinkius.com/mcp/simple-fatoora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
