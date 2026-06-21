# Ezus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ezus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ezus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ezus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Streamline travel agency operations via Ezus — manage projects, clients, suppliers, and invoices through your AI agent.

## Description
Connect your **Ezus** travel management account to any AI agent and take full control of your agency's workflows through natural conversation.

### What you can do

- **Project Management** — List, fetch, and upsert travel projects directly from the Ezus cloud
- **Client & Supplier CRM** — Query client details and manage your network of suppliers with ease
- **Product Catalog** — Access and inspect your travel products and packages stored in the Ezus catalog
- **Financial Overview** — List and inspect invoices to keep track of your agency's billing and financial status
- **User Profiling** — Retrieve the underlying credentials and profile information of your agent's API user

### How it works

1. Subscribe to this server
2. Enter your Ezus API Key, Email, and Password
3. Start managing your travel agency from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agents** — quickly find project details or client info without leaving your communication tools
- **Agency Managers** — monitor billing and project status through simple natural language queries
- **Operations Teams** — sync project and supplier data directly within your AI-powered workflow


## Available Tools
- **list_projects**: List all Ezus projects
- **list_suppliers**: List all Ezus suppliers
- **upsert_project**: Create or update an Ezus project
- **get_client**: Get a specific Ezus client by ID
- **get_invoice**: Get a specific Ezus invoice by ID
- **get_me**: Get current Ezus user profile
- **get_product**: Get a specific Ezus product by ID
- **get_project**: Get a specific Ezus project by ID
- **get_supplier**: Get a specific Ezus supplier by ID
- **list_clients**: List all Ezus clients
- **list_invoices**: List all Ezus invoices
- **list_products**: List all Ezus products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ezus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent travel projects on Ezus."

**🤖 AI Agent:**
> I've retrieved your projects. You have 'Summer in Paris' (ID: 789) and 'Tokyo Explorer' (ID: 456) currently active. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the details for client ID 12345."

**🤖 AI Agent:**
> Inspecting client 12345... This is 'John Doe', a frequent traveler with a preference for luxury stays. They are currently associated with the 'Swiss Alps Adventure' project.

---

**👤 You:**
> "Get all products available in the catalog."

**🤖 AI Agent:**
> Fetching catalog... I found 12 products including 'Safari Package', 'Guided City Tour', and 'Airport Transfer'. Which one should I inspect further?


## Installation & Usage

To install and use the **Ezus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ezus](https://vinkius.com/mcp/ezus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
