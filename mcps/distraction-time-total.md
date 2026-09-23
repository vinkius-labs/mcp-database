# Distraction Time Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/distraction-time-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify lost productivity by aggregating distraction durations.

## Description
This MCP server provides tools to analyze and quantify time lost to interruptions. Use `get_total_distraction_time` to sum up all distraction events, `get_average_distraction_duration` to find the mean length of interruptions, and `get_distraction_frequency_metrics` to see how often distractions occur in specific time buckets. It also includes `validate_distraction_data` to ensure your recorded durations are consistent and valid for analysis.


## Available Tools (4)
- **get_average_distraction_duration**: Determines the typical length of a distraction event
- **get_distraction_frequency_metrics**: Provides a breakdown of how many distractions occurred within specific time buckets
- **get_total_distraction_time**: Calculates the total amount of time lost to distractions
- **validate_distraction_data**: Checks the integrity and sanity of a set of distraction recordings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Distraction Time Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total time lost if I had distractions of 5, 10, and 15 minutes?"

**🤖 AI Agent:**
> The total time lost is 30 minutes across 3 distraction events.

---

**👤 You:**
> "What was the average distraction length for 2, 4, and 6 minutes?"

**🤖 AI Agent:**
> The average distraction duration is 4 minutes.

---

**👤 You:**
> "Check if these distraction durations are valid: [10, 20, -5]"

**🤖 AI Agent:**
> The data is invalid because it contains a negative duration.


## ❓ FAQ

**Q: How do I calculate my total lost time?**
You can use the `get_total_distraction_time` tool by providing an array of all your recorded distraction durations.

**Q: Can I see how frequent my distractions are?**
Yes, the `get_distraction_frequency_metrics` tool allows you to group distractions into specific time buckets to see patterns.

**Q: How can I check if my distraction data is valid?**
The `validate_distraction_data` tool checks the integrity of your data to ensure all durations are positive and numeric.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/distraction-time-total](https://vinkius.com/en/ai-agent-connect/distraction-time-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Distraction Time Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `distraction-time-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Distraction Time Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "distraction-time-total": {
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
