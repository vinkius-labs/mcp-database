# Enterprise Deal Velocity Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-deal-velocity-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [revenue-operations](../categories/revenue-operations.md)

Calculate sales velocity and identify revenue acceleration opportunities.

## Description
This MCP server provides analytical tools to measure sales efficiency. Use `calculate_velocity` to determine monthly revenue flow from high-level pipeline metrics. For granular accuracy, `calculate_weighted_velocity` accounts for deal-specific win probabilities and stage aging. You can also use `analyze_segment_velocity` to compare performance across Enterprise, Mid-Market, and SMB tiers, or `identify_acceleration_opportunities` to find specific levers to increase revenue.


## Available Tools (4)
- **analyze_segment_velocity**: Breaks down velocity metrics by specific business segments
- **calculate_velocity**: Calculates the core monthly sales velocity based on high-level pipeline metrics
- **calculate_weighted_velocity**: Provides a more accurate velocity calculation by accounting for specific probabilities of deals at different stages
- **identify_acceleration_opportunities**: Detects specific areas where the sales process can be optimized to increase revenue flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Deal Velocity Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my monthly sales velocity if I have a $1,000,000 pipeline, a 20% win rate, an average deal size of $50,000, and a 60-day sales cycle?"

**🤖 AI Agent:**
> Your monthly sales velocity is $166,666.67.

---

**👤 You:**
> "Analyze my segment velocity for these deals: [{'value': 50000, 'winRate': 0.3, 'salesCycleDays': 30, 'segment': 'SMB'}, {'value': 200000, 'winRate': 0.15, 'salesCycleDays': 90, 'segment': 'Enterprise'}]"

**🤖 AI Agent:**
> The SMB segment has a velocity of $5,000.00 and the Enterprise segment has a velocity of $33,333.33.

---

**👤 You:**
> "Identify acceleration opportunities if my current win rate is 15%, deal size is $40,000, and cycle is 50 days, but my targets are 20% win rate, $50,000 deal size, and 40 days cycle."

**🤖 AI Agent:**
> Opportunities identified: Increase Win Rate, Increase Average Deal Size, and Shorten Sales Cycle. Potential velocity increase: $125,000.00.


## ❓ FAQ

**Q: How is sales velocity calculated?**
The core velocity is calculated by multiplying the pipeline value, win rate, and average deal size, then dividing by the sales cycle duration.

**Q: Can I see velocity by business segment?**
Yes, the `analyze_segment_velocity` tool allows you to break down metrics by segments like Enterprise, Mid-Market, and SMB.

**Q: How do I find ways to improve my sales process?**
Use the `identify_acceleration_opportunities` tool to compare your current metrics against target benchmarks and find optimization levers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-deal-velocity-metrics](https://vinkius.com/ai-agent-connect/enterprise-deal-velocity-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Deal Velocity Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-deal-velocity-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Deal Velocity Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-deal-velocity-metrics": {
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
