# Happyrobot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/happyrobot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Connect Happyrobot to any AI agent via MCP.



## Available Tools (1)
- **happyrobot_info**: Get information from Happyrobot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Happyrobot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger a check-call for load #1045."

**🤖 AI Agent:**
> I have triggered an automated check-call to the carrier assigned to load #1045. I will update the status once the call is complete and the driver's location is confirmed.

---

**👤 You:**
> "List all pending inbound requests from carriers today."

**🤖 AI Agent:**
> There are currently 4 pending inbound requests from carriers regarding load statuses. You can find their details in the active communications dashboard.

---

**👤 You:**
> "Summarize the call logs for the past 24 hours."

**🤖 AI Agent:**
> Over the last 24 hours, Happyrobot successfully completed 125 check-calls and received 42 inbound queries. 94% of outbound calls resulted in successful status updates.


## ❓ FAQ

**Q: What is Happyrobot?**
Happyrobot is an AI-powered voice and communication platform specifically built for the logistics and freight industry, designed to automate routine check-calls, status updates, and supply chain operations.

**Q: Where can I find my API credentials?**
You can find your API credentials in the Happyrobot dashboard under the Developer or Integrations settings. You will need your API key to authenticate requests.

**Q: Can I trigger automated calls via this integration?**
Yes, you can initiate automated outbound check-calls and manage voice interactions through the API by specifying the target load or carrier information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/happyrobot](https://vinkius.com/mcp/happyrobot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Happyrobot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `happyrobot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Happyrobot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "happyrobot": {
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
