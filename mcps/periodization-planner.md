# Periodization Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/periodization-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured athletic training macrocycles based on periodization models and target event timelines.

## Description
The Periodization Planner is a mathematical engine designed for athletes and coaches to structure long-term training plans. By providing a target event date, the number of weeks available, and a chosen periodization model (such as Linear, Daily Undulating, Weekly Undulating, or Block Periodization), the tool calculates a complete macrocycle breakdown. It determines the division of phases including Preparatory, Specific, Competitive, and Tapering, along with mesocycles. Users can also use `get_phase_attributes` to retrieve specific training focuses like volume and intensity for each phase, and `generate_weekly_load_progression` to obtain a week-by-week breakdown of relative training load percentages. This ensures physiological adaptation is maximized through systematic planning.


## Available Tools (3)
- **generate_weekly_load_progression**: Provides a week-by-week breakdown of the relative training load
- **get_phase_attributes**: Retrieves the specific training focus, target volume, and target intensity for a given phase
- **calculate_macrocycle_structure**: Determines how the total available time should be divided into phases and mesocycles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Periodization Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a training structure for an event on 2025-12-01 with 24 weeks available using the Linear model."

**🤖 AI Agent:**
> The macrocycle is divided into four phases: Preparatory (Weeks 1-10), Specific (Weeks 11-17), Competitive (Weeks 18-22), and Tapering (Weeks 23-24).

---

**👤 You:**
> "What is the training focus for the Preparatory phase in a Block Periodization plan?"

**🤖 AI Agent:**
> In the Preparatory phase, the target volume is High, the target intensity is Low, and the primary focus is building an aerobic base and work capacity.

---

**👤 You:**
> "Show me the weekly load progression for 12 weeks using Daily Undulating Periodization."

**🤖 AI Agent:**
> Week 1: 75%, Week 2: 80%, Week 3: 70%, Week 4: 85%, Week 5: 75%, Week 6: 80%, Week 7: 70%, Week 8: 85%, Week 9: 75%, Week 10: 80%, Week 11: 60%, Week 12: 50%.


## ❓ FAQ

**Q: What periodization models are supported?**
The engine supports Linear, Daily Undulating, Weekly Undulating, and Block Periodization models.

**Q: How do I know the training intensity for a specific phase?**
You can use the `get_phase_attributes` tool to retrieve qualitative descriptions of volume, intensity, and primary physiological focus for any given phase.

**Q: Can I see a week-by-week breakdown of my training load?**
Yes, the `generate_weekly_load_progression` tool provides an array containing the week number and the relative load percentage for your entire macrocycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/periodization-planner](https://vinkius.com/mcp/periodization-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Periodization Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `periodization-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Periodization Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "periodization-planner": {
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
