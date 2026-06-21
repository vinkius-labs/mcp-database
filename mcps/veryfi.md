# Veryfi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/veryfi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/veryfi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/veryfi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Automate document OCR and data extraction via Veryfi — process receipts, invoices, business cards, bank statements, and tax forms directly from your AI agent.

## Description
Connect your **Veryfi** account to any AI agent and automate document data extraction with human-level accuracy in seconds.

### What you can do

- **Receipts & Invoices** — Process and extract structured line-by-line data from financial documents using `process_documents`
- **Tax Forms & Bank Statements** — Parse complex financial forms like W-2s, W-9s, W-8BEN-Es, and bank statements with dedicated tools like `process_w2s` and `process_bank_statements`
- **Business Cards & Checks** — Extract contact details and check metadata instantly using `process_business_cards` and `process_checks`
- **Custom Blueprints** — Process any unstructured document using custom blueprints with `process_any_document`
- **Document Management** — Retrieve, update, and delete processed documents securely using `get_documents`, `update_documents`, and `delete_documents`

### How it works

1. Subscribe to this server
2. Enter your Veryfi Client ID, Username, API Key, and Client Secret
3. Start processing documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — Automate expense management, invoice processing, and bank reconciliation without manual data entry
- **Developers** — Integrate advanced OCR and document parsing directly into your development workflows and AI agents
- **Operations Managers** — Streamline tax document collection and business card sorting automatically


## Available Tools
- **delete_bank_statements**: Delete a bank_statements
- **delete_business_cards**: Delete a business_cards
- **delete_checks**: Delete a checks
- **delete_contracts**: Delete a contracts
- **delete_documents**: Delete a documents
- **delete_parse_documents**: Delete a parse_documents
- **delete_w2s**: Delete a w2s
- **delete_w8ben_e**: Delete a w8ben_e
- **delete_w9s**: Delete a w9s
- **get_bank_statements**: Get a specific bank_statements by ID
- **get_business_cards**: Get a specific business_cards by ID
- **get_checks**: Get a specific checks by ID
- **get_contracts**: Get a specific contracts by ID
- **get_documents**: Get a specific documents by ID
- **get_parse_documents**: Get a specific parse_documents by ID
- **get_w2s**: Get a specific w2s by ID
- **get_w8ben_e**: Get a specific w8ben_e by ID
- **get_w9s**: Get a specific w9s by ID
- **list_bank_statements**: List bank_statements
- **list_business_cards**: List business_cards
- **list_checks**: List checks
- **list_contracts**: List contracts
- **list_documents**: List documents
- **list_parse_documents**: List parse_documents
- **list_w2s**: List w2s
- **list_w8ben_e**: List w8ben_e
- **list_w9s**: List w9s
- **process_bank_statements**: Process a new bank_statements
- **process_business_cards**: Process a new business_cards
- **process_checks**: Process a new checks
- **process_contracts**: Process a new contracts
- **process_documents**: Process a new documents
- **process_parse_documents**: Process a new parse_documents
- **process_w2s**: Process a new w2s
- **process_w8ben_e**: Process a new w8ben_e
- **process_w9s**: Process a new w9s
- **update_bank_statements**: Update a bank_statements
- **update_business_cards**: Update a business_cards
- **update_checks**: Update a checks
- **update_contracts**: Update a contracts
- **update_documents**: Update a documents
- **update_parse_documents**: Update a parse_documents
- **update_w2s**: Update a w2s
- **update_w8ben_e**: Update a w8ben_e
- **update_w9s**: Update a w9s
- **add_webhook**: Add a pending webhook
- **classify_document**: Classify a document into a specific type
- **confirm_webhook**: Confirm a pending webhook
- **create_client_key**: Create a new API key
- **delete_any_document**: Delete any document
- **delete_client_key**: Remove a client key
- **get_any_document**: Get any document by ID
- **list_any_documents**: List any documents
- **list_client_keys**: Retrieve client keys list
- **list_webhooks**: Get configured webhooks
- **process_any_document**: Process any unstructured document using a blueprint
- **reset_client_keys**: Regenerate all API keys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Veryfi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Process this receipt URL: https://example.com/receipt.jpg"

**🤖 AI Agent:**
> I've processed the receipt. Here are the details:
- **Vendor**: Tech Supplies Inc.
- **Total**: $124.50
- **Tax**: $10.20
- **Date**: 2023-10-25
Would you like me to list the line items?

---

**👤 You:**
> "Extract data from this bank statement: https://example.com/statement.pdf"

**🤖 AI Agent:**
> I've analyzed the bank statement. Here is the summary:
- **Bank**: Chase Bank
- **Account Number**: *******1234
- **Beginning Balance**: $5,430.00
- **Ending Balance**: $6,120.00
- **Statement Period**: Oct 1 - Oct 31, 2023

---

**👤 You:**
> "Process this driver's license using the 'us_driver_license' blueprint: https://example.com/license.png"

**🤖 AI Agent:**
> Using the 'us_driver_license' blueprint, I extracted the following:
- **Name**: Jane Doe
- **License Number**: D1234567
- **State**: CA
- **Expiration Date**: 2028-05-12
- **Date of Birth**: 1990-01-01


## Installation & Usage

To install and use the **Veryfi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veryfi](https://vinkius.com/mcp/veryfi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
