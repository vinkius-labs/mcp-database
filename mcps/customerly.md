# Customerly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customerly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Combine live chat, email marketing, and customer surveys in one platform that helps SaaS companies grow and retain users.

## Description
Connect your **Customerly** account to any AI agent and take full control of your customer success and support workflows through natural conversation.

### What you can do

- **User & Lead Orchestration** — Create and manage customer profiles programmatically, including synchronizing custom attributes and managing lifecycle status
- **Conversation Intelligence** — Access complete chat histories and retrieve detailed interaction metadata to provide high-fidelity context for support
- **Engagement Tracking** — Monitor active chat sessions and customer interactions in real-time to optimize your team's response strategy
- **Audience Segmentation** — Programmatically add or remove tags for users and leads to maintain a structured and personalized communication ecosystem
- **Record Management** — Securely delete user records or update contact identification to ensure your database remains perfectly coordinated and compliant

### How it works

1. Subscribe to this server
2. Retrieve your **API Access Token** from the Customerly dashboard (Settings > API)
3. Start managing your customer relationships from Claude, Cursor, or any MCP client

No more manual ticket searching or digging through user tables in the portal. Your AI acts as your dedicated success engineer and support coordinator.

### Who is this for?

- **Customer Success Teams** — instantly retrieve user profiles and summary interaction histories using natural language commands
- **Marketing Automation Leads** — automate the tagging and segmentation of new leads without leaving your workspace
- **Product Managers** — track user engagement and sync backend metadata through simple AI queries


## Available Tools (8)
- **get_conversation**: Get details of a specific conversation
- **add_tag**: Provide tag name and contact identification.

Add a tag to a contact
- **create_update_lead**: Create or update a lead
- **create_update_user**: Provide email and optionally user_id, name, and attributes.

Create or update a user
- **delete_user**: Delete a user
- **list_conversations**: List all conversations
- **list_users**: List all users
- **remove_tag**: Remove a tag from a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customerly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in my Customerly account."

**🤖 AI Agent:**
> I've retrieved your user directory. You currently have 5 registered users, including 'John Doe' (ID: usr_123) and 'Sarah Smith'. Would you like the interaction history for any of them?

---

**👤 You:**
> "Create a new lead for 'Jane Smith' at 'jane@example.com'."

**🤖 AI Agent:**
> Lead registered! Jane Smith has been added to Customerly. I've initialized her profile and she is now available for chat sessions and tagging.

---

**👤 You:**
> "Show me the transcript for conversation ID 'conv_456'."

**🤖 AI Agent:**
> Fetching transcript... Conversation conv_456 features a discussion about 'Pricing Plans' from 2 hours ago. Agent Sarah provided the link to the Pro plan. Would you like to add an internal note?


## ❓ FAQ

**Q: How do I find my Customerly Access Token?**
Log in to your Customerly dashboard, navigate to **Settings** > **API**, and generate or copy your Access Token.

**Q: Can I read full chat histories?**
Yes! The `get_conversation` tool retrieves the detailed message log and interaction metadata for any specific conversation ID.

**Q: How do I add tags to a user?**
Use the `add_tag` tool and provide the tag name along with either the user's `email` or their unique `user_id`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customerly](https://vinkius.com/mcp/customerly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customerly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customerly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customerly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customerly": {
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
