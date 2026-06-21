# Eversign (Cloud Electronic Signature) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eversign-cloud-electronic-signature)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eversign-cloud-electronic-signature-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eversign-cloud-electronic-signature-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage electronic signatures via Eversign — list businesses, create documents, and handle templates directly from any AI agent.

## Description
Connect your **Eversign** account to any AI agent to streamline your document signing workflows through natural conversation.

### What you can do

- **Business Management** — List all businesses associated with your account to retrieve the necessary Business IDs for operations.
- **Document Creation** — Generate new documents for signature from scratch, including custom files, signers, and specific fields.
- **Template Automation** — Create reusable templates or generate new signing requests from existing template hashes instantly.
- **Sandbox Testing** — Use the sandbox mode to test your document workflows without creating legally binding contracts.
- **Embedded Signing** — Create drafts specifically configured for iFrame or embedded signing environments.

### How it works

1. Subscribe to this server
2. Enter your Eversign API Access Key
3. Start managing your digital contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & HR Teams** — quickly send out NDAs, offer letters, or contracts without leaving your workspace
- **Sales Operations** — automate the generation of sales agreements from templates directly from your CRM context
- **Developers** — test e-signature integrations using the sandbox mode and inspect business structures via API


## Available Tools
- **create_document**: Can also be used to create reusable templates or generate documents from templates.

Create a new document, create a template, or use an existing template
- **list_businesses**: Use this to find the business_id required for document operations.

List all businesses associated with your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eversign (Cloud Electronic Signature)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all businesses in my Eversign account."

**🤖 AI Agent:**
> I've retrieved your business profiles. You have access to 'Global Logistics Ltd' (ID: 54321) and 'Creative Agency' (ID: 98765). Which business ID would you like to use for your document?

---

**👤 You:**
> "Create a test document in sandbox mode for business 54321 with a signer named Alice."

**🤖 AI Agent:**
> I've initiated the document creation in sandbox mode for business 54321. The document has been prepared for Alice. Since this is sandbox mode, it will not be legally binding.

---

**👤 You:**
> "Generate a document from template 'abc123hash' for business 98765."

**🤖 AI Agent:**
> Processing template 'abc123hash'... I have successfully generated a new document for business 98765 based on your template. Would you like to check the status of the signers?


## Installation & Usage

To install and use the **Eversign (Cloud Electronic Signature)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eversign-cloud-electronic-signature](https://vinkius.com/mcp/eversign-cloud-electronic-signature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
