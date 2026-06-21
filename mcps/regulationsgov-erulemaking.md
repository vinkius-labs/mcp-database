# Regulations.gov (eRulemaking) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regulationsgov-erulemaking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/regulationsgov-erulemaking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/regulationsgov-erulemaking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Access US federal regulations, search documents, public comments, and dockets directly from agencies like the EPA and FAA.

## Description
Connect your AI agent to the **Regulations.gov** database to navigate the US federal rulemaking process with ease. This server provides direct access to the eRulemaking Program, allowing you to monitor legislative changes and public discourse across hundreds of federal agencies.

### What you can do

- **Document Search** — Find rules, proposed rules, and notices using keywords, agency IDs, or specific posting dates.
- **Public Comments** — Retrieve and analyze public feedback submitted to federal agencies to understand community sentiment on specific regulations.
- **Docket Tracking** — Access complete docket folders containing all supporting materials and related documents for specific rulemaking actions.
- **Deep Metadata** — Fetch detailed information about document types, comment periods, and modification histories to stay ahead of regulatory deadlines.

### How it works

1. Subscribe to this server
2. Enter your Regulations.gov API Key
3. Start querying federal data from Claude, Cursor, or any MCP-compatible client

Stay informed about government transparency and regulatory updates without manually browsing complex government portals. Your AI acts as a specialized regulatory analyst.


## Available Tools
- **get_comment**: Get details for a specific comment
- **get_docket**: Get details for a specific docket
- **get_document**: Get details for a specific document
- **search_comments**: Search public comments
- **search_dockets**: Search dockets
- **search_documents**: Search for documents (rules, notices, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regulations.gov (eRulemaking)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent documents from the EPA related to 'air quality' posted after 2024-01-01."

**🤖 AI Agent:**
> I've found several documents from the EPA regarding air quality. The most recent is a Proposed Rule (ID: EPA-HQ-OAR-2023-0014) regarding emission standards. Would you like to see the full details or the associated comments?

---

**👤 You:**
> "Find public comments submitted for document ID FAA-2023-1234-0001."

**🤖 AI Agent:**
> I've retrieved 15 public comments for that FAA document. They range from industry feedback to individual pilot concerns. I can summarize the top comments or fetch the full text of a specific one for you.

---

**👤 You:**
> "Get the full details for docket folder CMS-2024-0005."

**🤖 AI Agent:**
> Accessing docket CMS-2024-0005... This docket is managed by the Centers for Medicare & Medicaid Services and contains 3 supporting documents and 1 final rule. The last modification was on 2024-02-15.


## Installation & Usage

To install and use the **Regulations.gov (eRulemaking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regulationsgov-erulemaking](https://vinkius.com/mcp/regulationsgov-erulemaking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
