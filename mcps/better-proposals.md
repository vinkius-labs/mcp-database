# Better Proposals MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/better-proposals)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Create and manage professional proposals via Better Proposals — list proposals, contacts, and templates directly from any AI agent.

## Description
Connect your **Better Proposals** account to any AI agent and orchestrate your sales documents and proposal workflows through natural conversation.

### What you can do

- **Proposal Management** — List, retrieve, and create professional proposals to close deals faster.
- **Contact & Company Oversight** — Manage your CRM data, including contacts and companies, for targeted document delivery.
- **Template Discovery** — Access and list your saved proposal templates for consistent and fast document creation.
- **Sales Analytics** — Retrieve performance data and status updates for all your outgoing proposals.
- **Account Integration** — Verify user profiles and organization settings directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Better Proposals API Key
3. Start closing more deals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — quickly check proposal statuses and create new documents without leaving their workflow tools.
- **Account Managers** — retrieve client and company details for proposal customization.
- **Small Business Owners** — automate proposal management and follow-ups using natural language.


## Available Tools (10)
- **create_contact**: Create a new contact
- **create_proposal**: Create a new proposal
- **get_analytics**: Retrieve proposal analytics
- **get_company**: Get specific company details
- **get_contact**: Get specific contact details
- **get_proposal**: Get specific proposal details
- **list_companies**: List all companies
- **list_contacts**: List all contacts
- **list_proposals**: List all proposals
- **list_templates**: List all proposal templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Better Proposals** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all proposals currently waiting for signature."

**🤖 AI Agent:**
> I've retrieved your pending proposals. You have 3 documents waiting for signature: 'Website Redesign' (ID: prop_1), 'SEO Audit Q1' (ID: prop_2), and 'Logo Design' (ID: prop_3).

---

**👤 You:**
> "Create a new contact: John Doe, email john@example.com."

**🤖 AI Agent:**
> I've successfully created 'John Doe' as a new contact in your account (ID: con_99283). Would you like to associate them with a company?

---

**👤 You:**
> "Show me my last 5 proposal templates."

**🤖 AI Agent:**
> Retrieving templates... I found 5 templates, including 'Modern SaaS Proposal', 'Consulting Agreement', and 'Creative Agency Services'. Which one would you like to use for your next document?


## ❓ FAQ

**Q: Can I see if a client has opened my proposal using the agent?**
Yes! Use the `get_proposal` tool with the Proposal ID. Your agent will fetch the latest status, which includes whether the proposal has been viewed, signed, or paid.

**Q: How do I list all my saved proposal templates?**
Simply ask the agent to `list_templates`. It will retrieve all the proposal templates available in your account for you to review and use.

**Q: Does the integration allow me to create a new contact?**
Yes! Use the `create_contact` action with the name and email. Your agent will register the new contact in your Better Proposals CRM instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-proposals](https://vinkius.com/mcp/better-proposals)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Better Proposals** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `better-proposals` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Better Proposals** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "better-proposals": {
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
