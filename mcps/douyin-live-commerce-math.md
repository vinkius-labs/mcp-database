# Douyin Live Commerce Math MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/douyin-live-commerce-math)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic economic funnel and GMV calculator for Douyin/TikTok live streams.

## Description
This MCP server provides a deterministic mathematical engine for analyzing the economic funnel of Douyin and TikTok live commerce. It allows creators to calculate key performance indicators such as unique clicks, total orders, Gross Merchandise Value (GMV), and net revenue. By using `calculate_stream_performance`, creators can evaluate past stream success. The `forecast_required_traffic` tool enables precise planning by determining the exact viewer count needed to hit specific revenue targets, while `analyze_funnel_efficiency` helps identify bottlenecks in the user journey from view to purchase.


## Available Tools (3)
- **analyze_funnel_efficiency**: Analyze the effectiveness of different stages in the user conversion journey
- **calculate_stream_performance**: Calculate total clicks, orders, GMV, net revenue, and engagement levels for a specific stream
- **forecast_required_traffic**: Determine how many viewers are needed to reach a target GMV goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin Live Commerce Math** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were my total clicks, orders, and GMV for a stream with 10,000 viewers, 30s average watch time, 3600s duration, 5% CTR, 10% conversion, 50 RMB AOV, and 5% commission?"

**🤖 AI Agent:**
> For that stream, you had 500 unique clicks, 50 total orders, a GMV of 2,500 RMB, and a net revenue of 2,375 RMB.

---

**👤 You:**
> "How many viewers do I need to reach 10,000 RMB GMV if my CTR is 5%, conversion rate is 10%, and average order value is 100 RMB?"

**🤖 AI Agent:**
> You will need 20,000 viewers to reach your target GMV of 10,000 RMB.

---

**👤 You:**
> "Analyze my funnel efficiency: 5,000 viewers, 8% CTR, and 5% conversion rate."

**🤖 AI Agent:**
> Your click efficiency is 8%, your purchase efficiency is 5%, and your overall conversion rate is 0.4%.


## ❓ FAQ

**Q: How do I calculate my expected revenue?**
You can use the `calculate_stream_performance` tool by providing your total viewers, watch time, click-through rate, conversion rate, and average order value.

**Q: Can I plan for a specific sales goal?**
Yes, use `forecast_required_traffic` to input your target GMV and current conversion metrics to find the necessary viewer count.

**Q: What is the engagement score?**
The engagement score is a percentage representing how much of the total stream duration viewers spent watching, calculated via `calculate_stream_performance`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/douyin-live-commerce-math](https://vinkius.com/ai-agent-connect/douyin-live-commerce-math)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Douyin Live Commerce Math** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `douyin-live-commerce-math` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Douyin Live Commerce Math** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "douyin-live-commerce-math": {
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
