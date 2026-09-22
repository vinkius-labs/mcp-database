# Coffee Caffeine Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coffee-caffeine-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate caffeine content in coffee servings and track daily intake.

## Description
This MCP server provides tools to monitor caffeine consumption. Use `calculate_serving_caffeine` to find the caffeine in a specific drink, `get_cumulative_intake` to see your total consumption, and `check_daily_limit_status` to ensure you stay within safe limits. It also allows you to `list_coffee_types` to see supported brewing methods.


## Available Tools (4)
- **calculate_serving_caffeine**: Calculate caffeine in a single coffee serving
- **check_daily_limit_status**: Check if a user is approaching or exceeding their daily caffeine limit
- **get_cumulative_intake**: Get total caffeine consumed by a user
- **list_coffee_types**: List all supported coffee types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coffee Caffeine Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much caffeine is in a 250ml americano?"

**🤖 AI Agent:**
> A 250ml americano contains 135mg of caffeine.

---

**👤 You:**
> "What is my total caffeine intake so far?"

**🤖 AI Agent:**
> Your total caffeine intake is 320mg.

---

**👤 You:**
> "Am I over my caffeine limit today?"

**🤖 AI Agent:**
> No, you have consumed 200mg and your limit is 400mg. You have 200mg remaining.


## ❓ FAQ

**Q: How do I know how much caffeine is in my espresso?**
You can use the `calculate_serving_caffeine` tool by providing the coffee type as 'espresso' and the volume in milliliters.

**Q: Can I track my total caffeine for the day?**
Yes, use `get_cumulative_intake` to see your total sum or `check_daily_limit_status` to see how much you have left before reaching your limit.

**Q: What coffee types are supported?**
You can call `list_coffee_types` to get a full list of all supported coffee identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coffee-caffeine-tracker](https://vinkius.com/en/ai-agent-connect/coffee-caffeine-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coffee Caffeine Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coffee-caffeine-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coffee Caffeine Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coffee-caffeine-tracker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
