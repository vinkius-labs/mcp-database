# Serviceform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serviceform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Convert website visitors with chatbots, forms, and booking widgets that generate leads and collect data without friction.

## Description
Connect your **Serviceform** account to any AI agent and take full control of your conversational marketing and lead orchestration through natural conversation. Serviceform provides a comprehensive platform for building chatbots, forms, and interactive multi-channel engagement, and this integration allows you to retrieve chat logs, manage flex spaces, and extract lead metadata directly from your chat interface.

### What you can do

- **Chat History & Insight Orchestration** — Retrieve and analyze chat logs with advanced time-based filters to understand customer intent programmatically.
- **Lead & CRM Management** — Access and monitor lead data captured through chatbots and forms to maintain a clear overview of your sales pipeline directly from the AI interface.
- **Space & Environment Control** — Manage 'flex spaces' and retrieve environment items to keep your service setup synchronized via natural language.
- **Bot & Form Discovery** — List all configured chatbots and active forms to monitor your conversion tools in real-time.
- **Operational Monitoring** — Track system statistics and manage lead profiles using simple AI commands to ensure your conversational tools are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Serviceform API Key from your dashboard settings
3. Start managing your conversational tools from Claude, Cursor, or any MCP-compatible client

No more manual logging or data exports. Your AI acts as a dedicated marketing analyst or lead manager.

### Who is this for?

- **Marketing Analysts** — quickly retrieve chat statistics and monitor lead quality without switching apps.
- **Sales Teams** — automate the extraction of lead contact info and conversation context via natural conversation.
- **Customer Support Managers** — streamline the retrieval of chat histories and monitor service spaces directly within the chat.


## Available Tools
- **get_lead**: Get lead details
- **get_space_items**: Get items for a specific space
- **list_chatbots**: List all configured chatbots
- **list_chats**: Pass criteria as a JSON string.

List chat histories
- **list_forms**: List all active forms
- **list_leads**: List leads captured
- **list_spaces**: List flex spaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serviceform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active flex spaces in my Serviceform account."

**🤖 AI Agent:**
> I've retrieved your spaces. You have 3 active environments: 'Sales Support', 'Marketing Hub', and 'General Inquiries'. Which one would you like to see items for?

---

**👤 You:**
> "Show me the last 3 leads from today."

**🤖 AI Agent:**
> Fetching latest leads... I found 3 new contacts including 'John Doe' (ID: 9912) and 'Alice Brown' (ID: 9913). Would you like to see the full profile for any of them?

---

**👤 You:**
> "List all my chatbots in Serviceform."

**🤖 AI Agent:**
> Retrieving chatbots... You have 5 configured bots including 'Site Helper', 'Pricing Assistant', and 'Lead Generator v2'. Should I check the statistics for any of them?


## ❓ FAQ

**Q: Can my AI automatically find the last 5 chat conversations received today?**
Yes! Use the `list_chats` tool. Provide a `startTime` (ISO 8601) and set a `limit` of 5, and your agent will return the most recent conversation logs instantly.

**Q: How do I list all leads captured across all my Serviceform tools?**
Simply ask the agent to run the `list_leads` action. It will retrieve the directory of leads, which you can then inspect individually using `get_lead`.

**Q: How do I find my Serviceform API Key?**
Log in to your Serviceform account and navigate to your integration settings or visit link.serviceform.com to generate your unique `sf-api-key`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serviceform](https://vinkius.com/mcp/serviceform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serviceform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `serviceform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serviceform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serviceform": {
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
