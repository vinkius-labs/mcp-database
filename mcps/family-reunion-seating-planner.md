# Family Reunion Seating Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-reunion-seating-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimizes family seating arrangements based on group size, accessibility, and social relationships.

## Description
This MCP server manages complex seating logistics for large family reunions. It uses tools like `suggest_seating_plan` to generate optimized layouts that respect hard constraints like table capacity and accessibility needs, while also considering social preferences. You can use `list_tables` to see available seating, `find_compatible_tables` to match specific groups to suitable spots, and `calculate_seating_score` to evaluate how well a plan satisfies family relationships.


## Available Tools (4)
- **calculate_seating_score**: 
- **find_compatible_tables**: 
- **list_tables**: 
- **suggest_seating_plan**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Reunion Seating Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you suggest a seating plan for my family reunion with 5 groups and 4 tables?"

**🤖 AI Agent:**
> I have generated an optimized seating plan. Group A is at Table 1, Group B is at Table 2, Group C is at Table 3, and Groups D and E are at Table 4. All capacity and accessibility constraints are met.

---

**👤 You:**
> "Which tables are available in the Garden area?"

**🤖 AI Agent:**
> In the Garden area, there are 3 tables available: Table ID Garden_01 (capacity 4), Garden_02 (capacity 6, accessible), and Garden_03 (capacity 4).

---

**👤 You:**
> "Check if Table 5 is suitable for a group of 4 that needs wheelchair access."

**🤖 AI Agent:**
> Yes, Table 5 is an accessible table with a capacity of 6, making it suitable for your group of 4.


## ❓ FAQ

**Q: How does the seating optimization work?**
The system uses the `suggest_seating_plan` tool to balance physical constraints like table capacity and accessibility with social preferences like affinity and friction between groups.

**Q: Can I filter tables by location?**
Yes, you can use the `list_tables` tool with a location filter to see only the tables available in a specific area or room.

**Q: How are accessibility needs handled?**
The system ensures accessibility by using `find_compatible_tables` to identify tables marked as accessible for groups that require them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-reunion-seating-planner](https://vinkius.com/en/ai-agent-connect/family-reunion-seating-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Reunion Seating Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-reunion-seating-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Reunion Seating Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-reunion-seating-planner": {
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
