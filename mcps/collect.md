# Collect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/collect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Enable your AI agent to manage data collection campaigns, send requests, and track submissions via the Collect API.

## Description
Connect your AI to **Collect**, the secure platform for gathering information and documents from clients.

### What you can do

- **Campaign Management** — List active data collection campaigns and check their completion status.
- **Request Sending** — Send new data requests to clients by email for KYC, onboarding, or compliance workflows.
- **Status Tracking** — Check the status of individual requests, view messages, and monitor completion.

### How it works

1. Add the Collect integration to your AI toolset.
2. Provide your API Key (from Settings > Integrations > API).
3. Manage your data collection workflows via natural language.

### Who is this for?

- **Compliance Teams** — Send and track KYC requests without switching to the Collect dashboard.
- **Accounting Firms** — Manage document collection campaigns for multiple clients from chat.
- **HR Teams** — Track onboarding document submissions and send reminders.


## Available Tools
- **send_message**: Send a message to a recipient regarding a specific request
- **create_request**: Send a new data collection request to a recipient
- **get_campaign**: Retrieve detailed information about a specific campaign
- **get_element_details**: Retrieve details of a specific element (field/block) in a request
- **get_request**: Retrieve details of a specific data request
- **get_team_info**: Retrieve information about your team in Collect
- **get_user_info**: Retrieve information about the currently authenticated user
- **list_campaigns**: Retrieve a list of all data collection campaigns in Collect
- **list_messages**: Retrieve a list of messages sent through Collect
- **list_requests**: Retrieve all data requests for a specific campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active data collection campaigns."

**🤖 AI Agent:**
> You have 3 active campaigns:
1. 'KYC Process' — 12/20 requests completed (60%)
2. 'Tax Documents 2025' — 45/50 requests completed (90%)
3. 'New Client Onboarding' — 3/8 requests completed (37%)
Want to send reminders for pending requests?

---

**👤 You:**
> "Send a data request to 'John Doe' (john@example.com) for the 'KYC Process' campaign."

**🤖 AI Agent:**
> Request sent to John Doe (john@example.com) for campaign 'KYC Process'. Request ID: req-7x2k. Status: pending. The client will receive an email with the secure link.

---

**👤 You:**
> "Send an automatic reminder to all clients with missing documents in the 'Tax 2025' campaign."

**🤖 AI Agent:**
> Done. Reminders were successfully sent to 5 pending clients in the 'Tax Documents 2025' campaign. The clients have been re-notified.


## ❓ FAQ

**Q: Where do I find my Collect API key?**
In the Collect dashboard, go to **Settings > Integrations > API** and generate a key. Copy it and paste it below.

**Q: Which authentication method does this use?**
This integration uses Basic Authentication with your API Key as the password.

**Q: Can I export requests as PDF?**
The API supports PDF exports. While this integration focuses on data management, you can retrieve the metadata needed to trigger an export.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/collect](https://vinkius.com/mcp/collect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `collect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collect": {
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
