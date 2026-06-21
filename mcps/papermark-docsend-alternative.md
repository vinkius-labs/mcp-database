# Papermark (Docsend Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/papermark-docsend-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/papermark-docsend-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/papermark-docsend-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Securely share documents, track engagement, and manage links with Papermark — the open-source DocSend alternative for your AI agent.

## Description
Connect your **Papermark** account to any AI agent to manage document sharing and analytics through natural conversation.

### What you can do

- **Document Management** — List all uploaded documents and upload new PDFs directly via base64 encoding
- **Link Creation** — Generate shareable links with custom slugs and security settings like passwords or email requirements
- **Engagement Analytics** — Retrieve detailed view statistics and engagement data for any specific link to see who is reading
- **Link Control** — Update link settings (like active status) or delete them entirely to revoke access instantly

### How it works

1. Subscribe to this server
2. Enter your Papermark API Key
3. Start managing your document workflows from Claude, Cursor, or any MCP-compatible client

No more manual link generation or checking dashboards to see if a client opened your deck. Your AI acts as your document operations assistant.

### Who is this for?

- **Founders & Sales Teams** — share pitch decks and sales collateral while tracking engagement in real-time
- **Marketers** — manage gated content and analyze which documents drive the most interest
- **Operations** — automate the creation of secure document links for clients or partners directly from your workflow


## Available Tools
- **create_link**: Create a new shareable link for a specific document
- **delete_link**: Permanently remove a shareable link
- **get_link_views**: Retrieve a list of views and engagement data for a specific link
- **list_documents**: List all documents in your Papermark account
- **update_link**: Modify the settings of an existing link
- **upload_document**: Upload a new document to Papermark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Papermark (Docsend Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my documents in Papermark."

**🤖 AI Agent:**
> I've retrieved your documents. You have 3 files: 'Q4_Investor_Deck.pdf' (ID: doc_1), 'Sales_Proposal.pdf' (ID: doc_2), and 'Product_Roadmap.pdf' (ID: doc_3).

---

**👤 You:**
> "Create a shareable link for document 'doc_1' with the slug 'pitch-deck' and require an email."

**🤖 AI Agent:**
> Link created successfully! You can share it at: papermark.io/view/pitch-deck. It is configured to require an email address before viewing.

---

**👤 You:**
> "Show me the view history and analytics for link ID 'link_999'."

**🤖 AI Agent:**
> Fetching analytics... Link 'link_999' has 15 total views. Most viewers spent an average of 2 minutes on page 4. Would you like a breakdown of the visitor emails?


## Installation & Usage

To install and use the **Papermark (Docsend Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/papermark-docsend-alternative](https://vinkius.com/mcp/papermark-docsend-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
