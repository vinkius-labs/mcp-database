# Get a Newsletter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/get-a-newsletter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Send professional newsletters to your audience with an email platform that makes list management and campaign tracking simple.

## Description
Connect your **Get a Newsletter** account to any AI agent and take full control of your email marketing workflows through natural conversation.

### What you can do

- **Subscriber Management** — List, create, update, or remove email contacts directly from the cloud
- **Contact Inspection** — Fetch detailed metadata for specific subscribers and verify their status
- **List Organization** — View all active subscriber lists and create new audience segments
- **Campaign Tracking** — Retrieve sent and drafted email campaigns along with their details

### How it works

1. Subscribe to this server
2. Enter your Get a Newsletter API Token
3. Start managing your audience from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated marketing assistant, ready to sync leads or pull campaign data without opening the browser.

### Who is this for?

- **Marketers** — instantly retrieve campaign statuses or audience lists without leaving your workflow
- **Engineering Teams** — add or check subscribers straight from the code editor to verify integrations
- **Founders** — automate CRM cross-referencing by letting the agent query your active contacts


## Available Tools (10)
- **get_contact**: Get details of a specific contact
- **get_list**: Get details of a specific list
- **list_campaigns**: List all campaigns
- **list_contacts**: List all contacts (subscribers)
- **list_lists**: List all subscriber lists
- **update_contact**: Update an existing contact
- **create_contact**: Create a new contact (subscriber)
- **create_list**: Create a new subscriber list
- **delete_contact**: Delete a contact
- **get_campaign**: Get details of a specific campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Get a Newsletter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our email campaigns on Get a Newsletter."

**🤖 AI Agent:**
> I've fetched your campaigns. You have 'Q4 Product Launch' (sent) and 'Weekly Digest' (draft). Would you like to inspect any of them?

---

**👤 You:**
> "Add a new subscriber john.doe@example.com with the name John Doe."

**🤖 AI Agent:**
> Success! I have created the new contact John Doe (john.doe@example.com) in your Get a Newsletter audience.

---

**👤 You:**
> "Check if we have a subscriber list available and create a new one called 'Beta Testers'."

**🤖 AI Agent:**
> I found one existing list named 'Default Audience'. I have now created the new list 'Beta Testers' successfully.


## ❓ FAQ

**Q: Can my AI automatically create a new subscriber and assign them a name?**
Yes! Use the `create_contact` tool with the email address and optional first/last name. Your agent will instantly register them in your Get a Newsletter database.

**Q: How do I check my previous or active email campaigns?**
Simply ask the agent to run the `list_campaigns` action. It will retrieve the latest sent, scheduled, or drafted email campaigns available in your account.

**Q: Can this integration delete my entire account or lists?**
No. The integration allows targeted deletions of specific contacts (`delete_contact`), but it does not expose destructive actions to wipe entire lists or account-level configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/get-a-newsletter](https://vinkius.com/mcp/get-a-newsletter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Get a Newsletter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `get-a-newsletter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Get a Newsletter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "get-a-newsletter": {
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
