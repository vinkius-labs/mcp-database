# Enterprise Sales Stage Conversion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-sales-stage-conversion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm](../categories/crm.md)

Analyze sales funnel efficiency, stage velocity, and optimization priorities.

## Description
This MCP server provides a specialized analytics engine for enterprise sales cycles. It connects AI agents to your sales data to calculate critical performance indicators. Use `get_funnel_conversion_metrics` to evaluate stage-to-stage efficiency, `get_stage_velocity_analysis` to identify bottlenecks where deals are stalling, and `get_dropout_analysis` to understand why deals are lost. Finally, use `get_optimization_priorities` to determine exactly where the sales team should focus efforts to maximize revenue based on combined friction metrics.


## Available Tools (4)
- **get_dropout_analysis**: Analyzes dropout records to find reason distribution and stage dropout counts
- **get_funnel_conversion_metrics**: Calculates conversion rates, total pipeline value, and average conversion rate
- **get_optimization_priorities**: Determines the top priority stage for optimization
- **get_stage_velocity_analysis**: Calculates stage velocities and identifies the bottleneck stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Sales Stage Conversion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current efficiency of our sales funnel at each stage?"

**🤖 AI Agent:**
> The current conversion rates are: Prospecting (45%), Discovery (30%), Proposal (60%), and Negotiation (25%). The average conversion rate across all stages is 40%.

---

**👤 You:**
> "Where are deals stalling in our sales process?"

**🤖 AI Agent:**
> The bottleneck stage is 'Solution Validation', where deals spend an average of 42 days before progressing or dropping out.

---

**👤 You:**
> "Why are we losing deals most frequently?"

**🤖 AI Agent:**
> The primary reason for deal dropouts is 'Budget Constraints', accounting for 40% of all lost deals, primarily occurring in the 'Negotiation' stage.


## ❓ FAQ

**Q: What metrics can I calculate with this server?**
You can calculate stage conversion rates, stage velocity (average days in stage), dropout reason distributions, and overall optimization priorities for your sales funnel.

**Q: How do I identify the main bottleneck in my sales process?**
Use the `get_stage_velocity_analysis` tool to find the stage with the highest average days spent, or use `get_optimization_priorities` for a holistic view of friction.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-sales-stage-conversion](https://vinkius.com/ai-agent-connect/enterprise-sales-stage-conversion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Sales Stage Conversion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-sales-stage-conversion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Sales Stage Conversion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-sales-stage-conversion": {
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
