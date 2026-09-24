# Boarding Group Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/boarding-group-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate boarding group requirements and passenger distribution.

## Description
This MCP server provides tools to manage aircraft boarding logistics by calculating how many groups are needed based on passenger volume and group capacity. Use `get_total_groups` to find the total number of groups, `get_group_distribution` for a detailed breakdown of passengers per group, `get_full_groups_count` to see how many groups are at maximum capacity, and `get_last_group_size` to identify the size of the final group.


## Available Tools (4)
- **get_full_groups_count**: Calculates how many boarding groups will be filled to their maximum capacity
- **get_group_distribution**: Provides a detailed breakdown of how many passengers will be in each group
- **get_last_group_size**: Identifies the number of passengers assigned to the very last boarding group
- **get_total_groups**: Determines how many distinct boarding groups are needed to accommodate all passengers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boarding Group Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many boarding groups are needed for 105 passengers with a group size of 20?"

**🤖 AI Agent:**
> You will need 6 boarding groups.

---

**👤 You:**
> "Show me the distribution for 50 passengers in groups of 15."

**🤖 AI Agent:**
> Group 1: 15 passengers, Group 2: 15 passengers, Group 3: 15 passengers, Group 4: 5 passengers.

---

**👤 You:**
> "How many groups will be completely full if I have 40 passengers and a group size of 10?"

**🤖 AI Agent:**
> 4 groups will be completely full.


## ❓ FAQ

**Q: How do I know how many groups are needed?**
You can use the `get_total_groups` tool to determine the exact number of sequential boarding groups required for your passenger count.

**Q: Can I see the specific number of passengers in each group?**
Yes, the `get_group_distribution` tool provides a complete list of every group and its corresponding passenger count.

**Q: How is the last group handled?**
The `get_last_group_size` tool identifies the number of passengers in the final group, which may be less than the maximum capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/boarding-group-counter](https://vinkius.com/en/ai-agent-connect/boarding-group-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Boarding Group Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boarding-group-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Boarding Group Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boarding-group-counter": {
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
