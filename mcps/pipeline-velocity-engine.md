# Pipeline Velocity Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-velocity-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate sales pipeline velocity, revenue forecasts, and identify bottlenecks.

## Description
This MCP server provides a suite of tools to analyze sales performance and revenue flow. Use `get_pipeline_velocity` to determine daily revenue generation, `get_revenue_forecast` to project future earnings, `identify_pipeline_bottlenecks` to find friction points in the funnel, and `analyze_pipeline_health` to assess overall stability. It helps sales leaders understand how quickly revenue moves through the pipeline and where to focus improvements.


## Available Tools (4)
- **analyze_pipeline_health**: Evaluates the stability and performance of the current pipeline
- **get_pipeline_velocity**: Calculates the daily revenue velocity of the sales pipeline
- **get_revenue_forecast**: Forecasts expected revenue over a specific timeframe
- **identify_pipeline_bottlenecks**: Identifies the primary factor restricting revenue flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Velocity Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current pipeline velocity if we have 50 deals at $10,000 each, a 20% win rate, and a 30-day cycle?"

**🤖 AI Agent:**
> Your current pipeline velocity is $3,333.33 per day.

---

**👤 You:**
> "Forecast our revenue for the next 90 days with a daily velocity of $5,000 and a 10% slippage factor."

**🤖 AI Agent:**
> The projected revenue for the next 90 days is $405,000.

---

**👤 You:**
> "Is my pipeline healthy? Velocity is $2,000, target is $2,500, win rate is 0.2, and average deal size is $5,000."

**🤖 AI Agent:**
> The pipeline status is Warning, as the current velocity is below the target.


## ❓ FAQ

**Q: How do I calculate my daily revenue rate?**
You can use the `get_pipeline_velocity` tool by providing your total opportunities, average deal size, win rate, and sales cycle length.

**Q: Can this tool help identify why my sales are slowing down?**
Yes, the `identify_pipeline_bottlenecks` tool analyzes your stage distribution and metrics to pinpoint if the issue is Conversion, Speed, or Volume/Flow.

**Q: How accurate are the revenue forecasts?**
Forecasts are generated using `get_revenue_forecast`, which accounts for a slippage factor to adjust for expected loss of momentum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-velocity-engine](https://vinkius.com/en/ai-agent-connect/pipeline-velocity-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Velocity Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-velocity-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Velocity Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-velocity-engine": {
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
