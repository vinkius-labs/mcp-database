# Bounsel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bounsel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bounsel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bounsel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your contract lifecycle via Bounsel — list documents, automate templates, and request signatures directly from any AI agent.

## Description
Connect your **Bounsel** CLM account to any AI agent and orchestrate your legal document workflows through natural conversation.

### What you can do

- **Document Oversight** — List and retrieve detailed metadata for all your generated contracts and legal documents.
- **Automated Drafting** — Create new documents instantly by merging your data with pre-configured smart templates.
- **Template Discovery** — List available templates and their required fields to ensure accurate data entry.
- **Signature Orchestration** — Initiate the digital signature process for any completed document.
- **Document Lifecycle** — Delete drafts or canceled documents to maintain a clean workspace.
- **Team Management** — Retrieve lists of users and account information to manage access.

### How it works

1. Subscribe to this server
2. Enter your Bounsel API Key
3. Start managing your contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Operations** — quickly check contract statuses and send for signature without navigating the portal.
- **Sales Teams** — generate customized NDAs and sales agreements straight from their workflow tools.
- **HR Managers** — automate employee contract generation using natural language.


## Available Tools
- **create_document**: Create a new document from a template
- **delete_document**: Delete a document
- **get_account_info**: Get company account info
- **get_document**: Get details of a specific document
- **get_template**: Get details of a specific template
- **list_documents**: List all CLM documents
- **list_templates**: List all smart templates
- **list_users**: List all account users
- **send_document**: Send a document for signature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bounsel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active documents in Bounsel."

**🤖 AI Agent:**
> I've retrieved your documents. You have 5 recent files, including 'NDA - Acme Corp' (ID: doc_1) and 'Employment Agreement - Jane' (ID: doc_2).

---

**👤 You:**
> "Send document doc_1 for signature."

**🤖 AI Agent:**
> Document 'doc_1' has been successfully sent for signature. The recipients will receive an email shortly.

---

**👤 You:**
> "List available smart templates."

**🤖 AI Agent:**
> Retrieving templates... You have 3 templates: 'Standard NDA' (ID: tpl_1), 'Sales Contract' (ID: tpl_2), and 'Offer Letter' (ID: tpl_3).


## Installation & Usage

To install and use the **Bounsel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bounsel](https://vinkius.com/mcp/bounsel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
