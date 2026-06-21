# Zenvia Conversion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenvia-conversion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Zenvia Conversion (Sirena) leads and messages directly through AI.

## Description
Connect your **Zenvia Conversion** (formerly Sirena) account to any AI agent to automate your sales and support workflows. Manage leads, send WhatsApp messages, and track interactions through natural conversation.

### What you can do

- **Lead Management** — Create and manage leads from multiple sources and track their conversion into prospects.
- **WhatsApp Messaging** — Send free-text messages to active conversations or initiate new ones using HSM templates.
- **Team Coordination** — List agents, groups, and labels to maintain a clear overview of your team's structure and assignments.
- **Interaction History** — View full interaction logs and histories for any prospect to maintain context across your sales pipeline.
- **Workflow Automation** — Streamline repetitive tasks like lead creation and follow-ups using natural language commands.

### How it works

1. Subscribe to this server
2. Enter your Zenvia Conversion API Key (from API Access app)
3. Start managing your sales conversations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — manage leads and WhatsApp conversations more efficiently without switching apps.
- **Support Agents** — quickly respond to customer queries and track interaction history.
- **Marketing Managers** — monitor lead acquisition and conversion rates across different groups and agents.


## Available Tools
- **create_lead**: You can include contact details and an initial message (comment).

Create a new lead in Zenvia Conversion
- **get_account**: Get account information
- **get_prospect**: Get detailed information about a specific prospect
- **list_agents**: List agents in the account
- **list_groups**: List agent groups
- **list_interactions**: List interactions for a prospect
- **list_labels**: List labels
- **list_prospects**: List all prospects in Zenvia Conversion
- **send_message**: Send a message to a prospect
- **send_template**: Send a message template (HSM) to a prospect


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenvia Conversion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active prospects in Zenvia Conversion."

**🤖 AI Agent:**
> I've retrieved your prospects. You have 12 active conversations. The most recent interactions are with 'John Doe' (Status: Hot) and 'Jane Smith' (Status: Follow-up needed).

---

**👤 You:**
> "Create a new lead for 'Alice' with phone +5511988887777."

**🤖 AI Agent:**
> Successfully created the lead for Alice. She has been added to your inbox and is now visible as a new prospect. Would you like to send her a template message?


## ❓ FAQ

**Q: What is the difference between a Lead and a Prospect?**
In Zenvia Conversion, a Lead is an initial contact entry. Once a lead is processed or created via the API, it becomes a Prospect in your CRM pipeline.

**Q: Can I start a WhatsApp conversation with a new number?**
Yes, but you must use an approved HSM template to initiate a new conversation. Free-text messages can only be sent to active conversations within the 24-hour window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenvia-conversion](https://vinkius.com/mcp/zenvia-conversion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zenvia Conversion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zenvia-conversion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zenvia Conversion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenvia-conversion": {
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
