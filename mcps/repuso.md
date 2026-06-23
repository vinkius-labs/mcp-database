# Repuso MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/repuso)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Collect and manage customer reviews effortlessly with Repuso AI agents.

## Description
### What you can do
- List and manage customer reviews and feedback.
- Send review invite requests to customers seamlessly.
- Manage sub accounts and users across your Repuso dashboard.

### How it works
1. Sign up for a Repuso account.
2. Obtain your API Token from the developer settings.
3. Connect your token to empower your AI Agent with Repuso.

### Who is this for?
Perfect for customer success teams, marketing professionals, and community managers who want to automate review collection and reputation management using AI agents.


## Available Tools (14)
- **bulk_create_invite_requests**: Bulk create invite requests
- **create_invite_request**: Create a new invite request
- **create_subaccount**: Create a new sub account
- **delete_invite_request**: Delete an invite request
- **delete_subaccount**: Delete a sub account
- **get_invite_request**: Get a specific invite request
- **get_review**: Get a specific review by ID
- **get_subaccount**: Get a specific sub account
- **get_user**: Get a specific user
- **list_invite_requests**: List invite requests in Repuso
- **list_reviews**: List reviews from Repuso
- **list_subaccounts**: List Repuso sub accounts
- **list_users**: List users in Repuso
- **update_subaccount**: Update a sub account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repuso** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest 10 reviews from my Repuso account."

**🤖 AI Agent:**
> Here are the latest reviews from your customers.

---

**👤 You:**
> "Send a review invite request to john@example.com."

**🤖 AI Agent:**
> The review invite request has been sent to john@example.com.

---

**👤 You:**
> "List all sub accounts managed under my Repuso profile."

**🤖 AI Agent:**
> Here is the list of all your sub accounts in Repuso.


## ❓ FAQ

**Q: Can the AI agent reply to reviews directly?**
Currently, the agent can list and read reviews. Replying may require manual action or using specific Repuso channels.

**Q: Is it possible to automate review invitations?**
Yes! You can ask the AI agent to create single or bulk invite requests to ask customers for feedback.

**Q: Can I manage multiple businesses with this integration?**
Absolutely. The agent has full access to list and manage your sub accounts within Repuso.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/repuso](https://vinkius.com/mcp/repuso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repuso** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repuso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repuso** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repuso": {
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
