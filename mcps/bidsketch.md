# Bidsketch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bidsketch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate proposal creation via Bidsketch — list proposals, clients, and templates directly from any AI agent.

## Description
Connect your **Bidsketch** account to any AI agent and orchestrate your professional proposal workflows through natural conversation.

### What you can do

- **Proposal Management** — List, retrieve, and create proposals to speed up your sales process.
- **Client Oversight** — Manage your client directory, including contact details and history.
- **Template Discovery** — Access and list your saved proposal templates for consistent document generation.
- **Fee Auditing** — List and verify the fees and line items associated with your proposals.
- **User Profiles** — Retrieve account and user information directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Bidsketch Subdomain and API Token
3. Start winning more bids from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers & Agencies** — quickly check proposal statuses and client details without manual dashboard navigation.
- **Sales Professionals** — create new proposals and clients straight from their workflow tools.
- **Consultants** — manage templates and audit proposal fees using natural language.


## Available Tools
- **create_client**: Create a new client
- **create_proposal**: Create a new proposal
- **get_client**: Get specific client details
- **get_proposal**: Get specific proposal details
- **get_user_details**: Get current user details
- **list_clients**: List all clients
- **list_fees**: List fees for a specific proposal
- **list_proposals**: List all proposals
- **list_templates**: List all proposal templates
- **update_proposal**: Update an existing proposal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bidsketch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active proposals in Bidsketch."

**🤖 AI Agent:**
> I've retrieved your proposals. You have 3 documents: 'Web Design Project' (ID: prop_1), 'Content Strategy' (ID: prop_2), and 'Marketing Audit' (ID: prop_3).

---

**👤 You:**
> "Find the contact ID for 'Acme Corp'."

**🤖 AI Agent:**
> I found one matching client: 'Acme Corporation' (ID: client_992). You can use this ID to create new proposals for them.

---

**👤 You:**
> "Show my last 5 proposal templates."

**🤖 AI Agent:**
> Retrieving templates... I found 5 templates, including 'Basic Design Services', 'Consulting Agreement', and 'SEO Retainer'. Which one would you like to use?


## ❓ FAQ

**Q: Can I check the status of a specific proposal using the agent?**
Yes! Use the `get_proposal` tool with the Proposal ID. Your agent will fetch the latest status, such as whether it has been viewed or accepted.

**Q: How do I list all my clients in Bidsketch?**
Simply ask the agent to `list_clients`. It will retrieve the directory of all companies and persons registered in your Bidsketch account.

**Q: Does the integration allow me to create a new client?**
Yes! Use the `create_client` action with the name and optionally the email. Your agent will register the new client in your Bidsketch account instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bidsketch](https://vinkius.com/mcp/bidsketch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bidsketch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bidsketch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bidsketch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bidsketch": {
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
