# Sales Target Progress Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sales-target-progress-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate sales progress, pacing status, performance tiers, and revenue forecasts.

## Description
This MCP server provides precise computational tools for sales performance analysis. It allows AI agents to evaluate how close a team or individual is to their goals using `get_achievement_summary`. It can determine if a sales trajectory is healthy via `get_pacing_status`, categorize performance levels with `get_performance_tier`, and predict end-of-period results using `get_projection_forecast`.


## Available Tools (4)
- **get_achievement_summary**: 
- **get_pacing_status**: 
- **get_performance_tier**: 
- **get_projection_forecast**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sales Target Progress Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current sales progress? My target is 100000 and I have sold 45000."

**🤖 AI Agent:**
> You have achieved 45% of your target. The remaining amount needed to reach your goal is 55,000.

---

**👤 You:**
> "Are we on track for our 50000 goal? We have 20000 in sales and 50% of the month has passed."

**🤖 AI Agent:**
> Yes, you are Ahead. Your progress is 40%, but since you are at the halfway point, your trajectory is performing well relative to the time elapsed.

---

**👤 You:**
> "Predict my final sales. Target is 120000, current sales are 60000, and 0.5 of the period is complete."

**🤖 AI Agent:**
> Your projected final sales are 120,000, which means you are on track to meet your target exactly.


## ❓ FAQ

**Q: How do I check if my sales team is on track?**
You can use the `get_pacing_status` tool. Provide the target amount, current actual sales, and the ratio of time elapsed to see if the status is Ahead, On Track, or Behind.

**Q: Can I predict my end-of-month revenue?**
Yes, the `get_projection_forecast` tool calculates the estimated final sales and the projected gap based on your current sales velocity.

**Q: What defines a 'High Performer'?**
Performance tiers are determined by `get_performance_tier`. Typically, reaching 100% or more of the target qualifies as a High Performer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sales-target-progress-engine](https://vinkius.com/en/ai-agent-connect/sales-target-progress-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sales Target Progress Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sales-target-progress-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sales Target Progress Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sales-target-progress-engine": {
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
