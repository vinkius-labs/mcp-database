# Running Split Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-split-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise running splits, cumulative times, and required paces.

## Description
A precision utility for runners to manage their training. Use `get_segment_split` to find the duration of a specific segment, `get_cumulative_splits` to generate a full pacing schedule, `get_pace_from_time` to determine the speed needed for a target finish, or `get_split_difference` to compare performance between different segments.


## Available Tools (4)
- **get_cumulative_splits**: Generates a list of elapsed times for every interval at a specific distance mark given a constant pace
- **get_pace_from_time**: Determines the pace required to cover a specific distance within a target total time
- **get_segment_split**: Calculates the time required to complete a single specific distance segment at a given pace
- **get_split_difference**: Calculates the difference in time between two different segments or two different paces over the same distance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Split Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take to run 5km at a pace of 5 minutes and 30 seconds?"

**🤖 AI Agent:**
> It will take 27:30 to complete 5km at that pace.

---

**👤 You:**
> "What pace do I need to run 10km in exactly 50 minutes?"

**🤖 AI Agent:**
> To finish 10km in 50 minutes, you need a pace of 5:00 per km.

---

**👤 You:**
> "What is the time difference between running 1km at 4:00 pace and 4:15 pace?"

**🤖 AI Agent:**
> The difference is 00:15.


## ❓ FAQ

**Q: How do I calculate my total time for a run?**
You can use `get_cumulative_splits` to see the total elapsed time at various distance marks based on your target pace.

**Q: Can I compare two different paces?**
Yes, use `get_split_difference` to find the exact time difference between two different paces over the same distance.

**Q: How do I find the pace needed for a specific goal time?**
Use `get_pace_from_time` by providing your target distance and the total time you want to achieve.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-split-calculator](https://vinkius.com/en/ai-agent-connect/running-split-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Split Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-split-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Split Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-split-calculator": {
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
