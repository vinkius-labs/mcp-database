# Short-Term Mine Planning Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/short-term-mine-planning-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Aligns equipment, grade, and stockpiles into actionable mining schedules.

## Description
This MCP server connects AI agents to mining operations by providing tools to manage short-term production. It allows for the generation of weekly and monthly schedules using `get_production_schedule`, identification of specific extraction areas via `get_dig_plan`, and precise ore blending calculations with `get_blending_strategy`. Additionally, users can monitor fleet efficiency through `get_equipment_utilization` and track material storage levels using `get_stockpile_status`.


## Available Tools (5)
- **get_blending_strategy**: Calculates how to mix ore from various sources to meet specific mineral concentration targets
- **get_dig_plan**: Identifies exactly where the equipment should be digging to meet production and grade needs
- **get_equipment_utilization**: Analyzes how well the available fleet is being used to meet the plan
- **get_production_schedule**: Provides a high-level overview of the planned mining activities over a specific timeframe
- **get_stockpile_status**: Monitors the current levels and contents of ore and waste stockpiles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Short-Term Mine Planning Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the production schedule for the upcoming month?"

**🤖 AI Agent:**
> The monthly schedule includes a total volume of 50,000 tons with an average grade of 1.2%, focusing on the North Bench extraction.

---

**👤 You:**
> "Where should we be digging next week to meet our targets?"

**🤖 AI Agent:**
> Next week, digging should focus on Location ID B-12 (20,000 tons, 1.5% grade) and Location ID C-04 (15,000 tons, 0.8% grade).

---

**👤 You:**
> "How much of Source A and Source B do I need to get a 1.0% grade?"

**🤖 AI Agent:**
> To achieve a 1.0% grade, you need a mix ratio of 60% from Source A and 40% from Source B.


## ❓ FAQ

**Q: How can I see the planned mining activities for next week?**
You can use the `get_production_schedule` tool and specify 'weekly' as the timeframe to see the planned activities.

**Q: How do I calculate the correct ore mix to hit a specific grade?**
Use the `get_blending_strategy` tool by providing your target grade and a list of available ore sources.

**Q: Can I check if a specific stockpile is full?**
Yes, use `get_stockpile_status` with the specific stockpile ID to check its current volume and capacity status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/short-term-mine-planning-optimizer](https://vinkius.com/en/ai-agent-connect/short-term-mine-planning-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Short-Term Mine Planning Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `short-term-mine-planning-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Short-Term Mine Planning Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "short-term-mine-planning-optimizer": {
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
