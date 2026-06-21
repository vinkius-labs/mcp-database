# Medallia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medallia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Customer experience management via Medallia — track surveys, responses, and experience programs.

## Description
Connect your **Medallia** experience management instance to any AI agent and take full control of your customer feedback and CX programs through natural conversation.

### What you can do

- **Survey Management** — List all customer surveys and fetch detailed configuration metadata
- **Feedback Monitoring** — Retrieve and search survey responses to understand customer sentiment in real-time
- **Program Oversight** — List and inspect experience management programs and their statuses
- **Alert Management** — Monitor and retrieve details for alerts triggered by specific customer feedback
- **User Inventory** — List authorized users and manage access within your Medallia instance

### How it works

1. Subscribe to this server
2. Enter your Medallia Base URL, Client ID, and Client Secret
3. Start managing your CX intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_alert**: Get details for a specific alert
- **get_program_details**: Get details for a specific program
- **get_response**: Get details for a specific response
- **get_survey**: Get details for a specific survey
- **list_alerts**: List feedback alerts
- **list_programs**: List experience management programs
- **list_responses**: List survey responses
- **list_surveys**: List all customer surveys
- **list_users**: List Medallia users
- **search_responses**: Search survey responses by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medallia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in Medallia."

**🤖 AI Agent:**
> Retrieving surveys... I found several active surveys including 'Post-Purchase Feedback' and 'Customer Satisfaction 2024'.

---

**👤 You:**
> "Search responses for the term 'disappointed'."

**🤖 AI Agent:**
> Searching... I identified 5 responses containing the term 'disappointed'. Would you like to see the details for these entries?

---

**👤 You:**
> "Show recent alerts from high-priority programs."

**🤖 AI Agent:**
> Querying alerts... There are 3 new alerts triggered by low NPS scores in the 'Premium Support' program.


## ❓ FAQ

**Q: How do I get my Medallia API credentials?**
You need to contact your Medallia administrator to enable the REST API and create an OAuth 2.0 application to receive your Client ID and Secret.

**Q: What survey data can I access?**
You can access survey configurations, individual responses, scores (like NPS), feedback comments, and metadata associated with each response.

**Q: Is my customer data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medallia](https://vinkius.com/mcp/medallia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Medallia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `medallia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Medallia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "medallia": {
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
