# Well Productivity Index Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-productivity-index-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate productivity indices, assess skin damage, and identify stimulation candidates.

## Description
This MCP server provides specialized tools for petroleum engineers to evaluate well performance. Use `calculate_well_productivity` to determine the productivity index (PI), specific PI, and ideal PI for a specific well. You can also use `evaluate_skin_impact` to quantify how much flow is lost due to near-wellbore damage, or `get_stimulation_priority` to rank wells that would benefit most from acidizing or fracturing. It connects your AI assistant directly to core reservoir engineering calculations.


## Available Tools (4)
- **get_stimulation_priority**: Ranks a set of wells based on their potential for productivity gain through stimulation
- **calculate_well_productivity**: Performs the primary productivity analysis for a single well
- **compare_wells_efficiency**: Compares multiple wells to determine which are performing best relative to their formation thickness
- **evaluate_skin_impact**: Isolates and quantifies the impact of the skin factor on the well's performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Productivity Index Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the productivity for a well with a flow rate of 500, reservoir pressure of 3000, bottomhole pressure of 2500, thickness of 50, and a skin factor of 2."

**🤖 AI Agent:**
> The productivity index is 100.0, the specific productivity index is 2.0, and the ideal productivity index is 150.0. The well is currently Damaged.

---

**👤 You:**
> "What is the impact of a skin factor if the actual PI is 80 and the ideal PI is 120?"

**🤖 AI Agent:**
> The skin factor impact is 40.0, resulting in a flow loss percentage of 33.33%, which is classified as Moderate damage.

---

**👤 You:**
> "Rank these wells for stimulation: Well_A (actual PI 50, ideal PI 100), Well_B (actual PI 80, ideal PI 85)."

**🤖 AI Agent:**
> The prioritized well is Well_A because it has a much higher potential for productivity gain.


## ❓ FAQ

**Q: How do I calculate the productivity of a specific well?**
You can use the `calculate_well_productivity` tool. Provide the flow rate, reservoir pressure, flowing bottomhole pressure, reservoir thickness, and the skin factor.

**Q: How can I identify which wells need stimulation?**
Use the `get_stimulation_priority` tool with a list of well analysis data to rank wells by their potential for productivity gain.

**Q: What is the purpose of the skin factor analysis?**
The `evaluate_skin_impact` tool quantifies the flow loss percentage and damage severity caused by the skin factor, helping to determine if a well is damaged or stimulated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-productivity-index-analyzer](https://vinkius.com/ai-agent-connect/well-productivity-index-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Productivity Index Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-productivity-index-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Productivity Index Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-productivity-index-analyzer": {
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
