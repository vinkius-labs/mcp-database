# Dubsado MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dubsado)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Run your creative business with proposal templates, contract signing, invoicing, and client scheduling in one seamless flow.

## Description
Connect your **Dubsado** account to any AI agent and take full control of your business operations and client lifecycle management through natural conversation.

### What you can do

- **Project Orchestration** — List and manage client projects programmatically, including updating statuses, tags, and retrieving detailed metadata
- **Billing & Invoicing** — Monitor financial records across projects and programmatically create new invoices with detailed line items and taxes
- **Contract Intelligence** — Access project agreements and e-signature documents to monitor signing progress and contract validity in real-time
- **Workflow Automation** — Programmatically trigger automated sequence templates for specific projects to coordinate onboarding and client journeys
- **Relationship CRM** — Access your complete directory of clients and leads to manage contact information and high-fidelity communication history

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Dubsado dashboard (Settings > Marcus / API)
3. Start managing your service-based business from Claude, Cursor, or any MCP client

No more manual project tracking or digging through CRM menus. Your AI acts as your dedicated business operations and client journey coordinator.

### Who is this for?

- **Creative Entrepreneurs** — instantly retrieve project details and manage client onboarding using natural language commands
- **Service-Based Teams** — monitor invoice statuses and trigger workflow sequences without leaving your workspace
- **Operations Leads** — automate deal registration and manage client contracts through simple AI queries


## Available Tools (12)
- **create_invoice**: Create a new invoice
- **create_project**: Create a new project
- **get_contract**: Get contract status and details
- **get_invoice**: Get details for a Dubsado invoice
- **get_project**: Get details for a Dubsado project
- **list_contacts**: List Dubsado contacts
- **list_contracts**: List project contracts
- **list_invoices**: List all invoices
- **list_projects**: List all Dubsado projects
- **list_workflow_templates**: List available workflow templates
- **update_project**: Update an existing project
- **apply_workflow**: Apply a workflow to a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dubsado** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects in Dubsado."

**🤖 AI Agent:**
> I've retrieved your active projects. You currently have 4 deals in progress, including 'Winter Wedding' (ID: proj_1) and 'Brand Identity Refresh'. Which one would you like to update?

---

**👤 You:**
> "Create a $200 invoice for project 'proj_1' for 'Design Services'."

**🤖 AI Agent:**
> Invoice generated! I've created the $200.00 invoice for 'Design Services' associated with project proj_1. The ID is 'inv_123'. Shall I send it to the client for you?

---

**👤 You:**
> "Show me the status of the contract for 'Winter Wedding'."

**🤖 AI Agent:**
> Checking contract... For 'Winter Wedding' (ID: proj_1), the contract was viewed by the client yesterday but is still 'Pending Signature'. Would you like me to send a follow-up reminder?


## ❓ FAQ

**Q: How do I find my API Key in Dubsado?**
Log in to your account, navigate to **Settings** > **Marcus (API)**, and generate your unique key for the integration.

**Q: Can I filter projects by specific statuses?**
Yes! Use the `list_projects` tool. You can find valid status IDs by checking your project funnel settings in the Dubsado UI.

**Q: Does it support creating invoices with multiple items?**
Absolutely. The `create_invoice` tool accepts a JSON array of items, allowing you to specify names, amounts, and descriptions for each line.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dubsado](https://vinkius.com/mcp/dubsado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dubsado** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dubsado` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dubsado** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dubsado": {
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
