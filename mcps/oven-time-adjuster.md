# Oven Time Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/oven-time-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Adjust cooking times by a specific percentage.

## Description
This MCP server provides precise tools to modify cooking durations based on oven performance or recipe requirements. Use `calculate_adjusted_time` to find new durations, `validate_adjustment_range` to ensure safety, `format_cooking_duration` for readable time strings, and `get_adjustment_summary` for a full breakdown of the change.


## Available Tools (4)
- **validate_adjustment_range**: Validate if a percentage adjustment is within safe cooking bounds
- **calculate_adjusted_time**: Calculate the new cooking time after applying a percentage adjustment
- **format_cooking_duration**: Format a duration in seconds into a human-readable string
- **get_adjustment_summary**: Get a summary of the cooking time adjustment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oven Time Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If my recipe says 30 minutes, what is the new time if I increase it by 20%?"

**🤖 AI Agent:**
> The new cooking time will be 36 minutes.

---

**👤 You:**
> "I need to reduce a 120 second cook time by 50%. What is the result?"

**🤖 AI Agent:**
> The adjusted cooking time is 60 seconds.

---

**👤 You:**
> "Show me a summary for a 45 minute cook time with a 10% increase."

**🤖 AI Agent:**
> Original duration: 45 minutes, Delta: 4.5 minutes, Final duration: 49.5 minutes.


## ❓ FAQ

**Q: How do I increase the cooking time?**
Provide a positive percentage to the `calculate_adjusted_time` tool. For example, use 10 to increase the time by 10%.

**Q: Can I decrease the cooking time?**
Yes, use a negative percentage. For example, -15 will reduce the cooking time by 15%.

**Q: How can I see a summary of the changes?**
You can use the `get_adjustment_summary` tool to see the original duration, the delta, and the final calculated time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/oven-time-adjuster](https://vinkius.com/en/ai-agent-connect/oven-time-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oven Time Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oven-time-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oven Time Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oven-time-adjuster": {
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
