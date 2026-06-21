# Adafruit IO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adafruit-io)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Adafruit IO feeds, data points, dashboards, and triggers.

## Description
# Adafruit IO

The Adafruit IO MCP Server allows AI agents to interact with your IoT data seamlessly.

### What you can do
- Retrieve feeds and specific data points.
- Access dashboards and groups.
- View active triggers.

### How it works
Connect your Adafruit IO account via your AIO Key to manage your Internet of Things hardware remotely.


## Available Tools
- **get_dashboard**: Get a specific dashboard
- **get_data**: Get a specific data point
- **get_feed**: Get a specific feed
- **get_group**: Get a specific group
- **get_trigger**: Get a specific trigger
- **list_dashboards**: List all dashboards
- **list_data**: List data for a specific feed
- **list_feeds**: List all Adafruit IO feeds
- **list_groups**: List all groups
- **list_triggers**: List all triggers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adafruit IO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my IoT feeds."

**🤖 AI Agent:**
> I retrieved your feeds. Here are the active ones: 'temperature', 'humidity'.

---

**👤 You:**
> "Get data from the temperature feed."

**🤖 AI Agent:**
> Here are your recent data points, including '22.5' and '23.1'.

---

**👤 You:**
> "Send a value of 75 to the 'humidity' feed."

**🤖 AI Agent:**
> Successfully created a new data point with value 75 in the 'humidity' feed.


## ❓ FAQ

**Q: Where do I find my AIO Key?**
Your AIO Key can be found by clicking the golden 'AIO Key' button on any page in Adafruit IO.

**Q: What access does this MCP need?**
It requires your Username and AIO Key to access your feeds and dashboards.

**Q: How do I send data to a feed?**
You can use the agent to create a new data point in a specific feed using the feed key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adafruit-io](https://vinkius.com/mcp/adafruit-io)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adafruit IO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adafruit-io` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adafruit IO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adafruit-io": {
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
