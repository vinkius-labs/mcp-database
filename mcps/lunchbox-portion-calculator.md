# Lunchbox Portion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lunchbox-portion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate total meal portions needed for school weeks based on child attendance.

## Description
This MCP server provides precise tools for school meal planning. It calculates total weekly portions, individual child requirements, and capacity limits. Use `get_weekly_portion_total` to determine the total food needed for a group, or `get_schedule_overlap_impact` to identify peak daily requirements based on specific attendance schedules.


## Available Tools (4)
- **get_capacity_planning**: Determines how many children can be fed given a fixed number of prepared portions and a specific school schedule
- **get_child_specific_requirements**: Determines how many portions a single specific child needs based on their individual attendance
- **get_schedule_overlap_impact**: Calculates the peak portion requirement for a single day based on a group schedule
- **get_weekly_portion_total**: Calculates the total number of food portions needed for all children for a standard school week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lunchbox Portion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many portions do I need for 10 children attending school 5 days a week with a 10% buffer?"

**🤖 AI Agent:**
> You will need 55 portions in total (50 base portions plus 5 buffer portions).

---

**👤 You:**
> "If I have 20 portions available and each child attends 4 days a week, how many children can I feed?"

**🤖 AI Agent:**
> You can fully support 5 children.

---

**👤 You:**
> "What is the peak requirement for an attendance schedule of [5, 8, 3, 2, 4]?"

**🤖 AI Agent:**
> The peak requirement is 8 portions, and the total weekly requirement is 22 portions.


## ❓ FAQ

**Q: How do I calculate the total portions for a whole week?**
You can use the `get_weekly_portion_total` tool by providing the number of children, the days they attend, and an optional buffer percentage.

**Q: Can I plan for peak daily demand?**
Yes, the `get_schedule_overlap_impact` tool allows you to input a daily attendance list to find the maximum portions needed on any single day.

**Q: How many children can I feed with a limited supply?**
Use the `get_capacity_planning` tool to determine the maximum number of children supported by your available portions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lunchbox-portion-calculator](https://vinkius.com/en/ai-agent-connect/lunchbox-portion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lunchbox Portion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lunchbox-portion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lunchbox Portion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lunchbox-portion-calculator": {
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
