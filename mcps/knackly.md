# Knackly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knackly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/knackly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/knackly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate legal and business documents from smart templates with conditional logic that adapts content to every unique situation.

## Description
Connect your **Knackly** account to any AI agent and automate document generation through natural conversation.

### What you can do

- **Template Management** — Browse templates and their field configurations
- **Document Generation** — Create documents from templates with field data
- **App Browsing** — List all Knackly apps and their configurations
- **Generation History** — Track document generation history and outputs

### How it works

1. Subscribe to this server
2. Enter your Knackly API Key
3. Start generating documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Teams** — generate contracts and legal documents from templates
- **Operations** — automate repetitive document creation
- **Sales** — create proposals and agreements on demand


## Available Tools
- **create_data_record**: Add a new record
- **get_record_details**: Get details for a specific record
- **list_catalogs**: List catalogs in a workspace
- **list_generated_documents**: List automated documents
- **list_data_models**: List models in a catalog
- **list_data_records**: List records for a model
- **list_webhooks**: List configured webhooks
- **list_workspaces**: List Knackly workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knackly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all apps and templates available for document generation."

**🤖 AI Agent:**
> Apps: 4. Legal (5 templates), Sales (3), HR (4), Finance (2). Legal templates: 'NDA — Mutual' (8 fields), 'Service Agreement' (12 fields), 'Employment Contract' (15 fields), 'Lease Agreement' (10 fields), 'IP Assignment' (6 fields). Most used: 'NDA — Mutual' (234 generations). Would you like to generate a document?

---

**👤 You:**
> "Generate an NDA for Acme Corp and show the required fields."

**🤖 AI Agent:**
> NDA — Mutual fields: 8. Party A Name (text, required): 'Our Company'. Party B Name: 'Acme Corp'. Effective Date: Apr 26, 2025. Duration (dropdown): 2 years. Governing Law: Delaware. Party A Signatory: 'CEO, Jane Smith'. Party B Signatory: 'CTO, John Doe'. Scope (textarea): 'Software development collaboration'. Document generated! ✅ NDA_AcmeCorp_20250426.pdf (3 pages). Download available.

---

**👤 You:**
> "Show document generation history for this month."

**🤖 AI Agent:**
> This month: 45 documents generated. By template: NDA (18), Service Agreement (12), Employment Contract (8), Lease Agreement (4), Other (3). By user: Sarah (15), Mike (12), Lisa (10), Others (8). Average generation time: 2.3 seconds. Success rate: 100%.


## Installation & Usage

To install and use the **Knackly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knackly](https://vinkius.com/mcp/knackly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
