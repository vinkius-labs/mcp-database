# Demo Day Conversion Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/demo-day-conversion-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze demo day success using a multi-stage funnel model and investor quality scoring.

## Description
This MCP server provides a specialized analytics engine to evaluate demo day effectiveness. It tracks the investor journey through a structured funnel: from initial attendance to signed deals. Use `get_funnel_metrics` to calculate conversion rates at every stage, `calculate_investor_quality` to assess the caliber of the investor pool based on tier engagement and thesis match, and `get_conversion_velocity` to measure the speed of the investment pipeline.


## Available Tools (3)
- **get_conversion_velocity**: How quickly and effectively are we moving investors through the pipeline?
- **get_funnel_metrics**: What were the conversion percentages at each stage of the demo day funnel?
- **calculate_investor_quality**: How high is the caliber of the investors engaged at this event?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Demo Day Conversion Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were the conversion percentages for my demo day with 50 attendees, 20 scheduled meetings, 10 follow-up meetings, 5 term sheets, and 3 deals closed?"

**🤖 AI Agent:**
> The meeting conversion rate was 40%, the term sheet conversion rate was 33.3%, and the closing rate was 60%.

---

**👤 You:**
> "How high is the caliber of my investors if I had 5 tier-1 engagements and a thesis match score of 0.8?"

**🤖 AI Agent:**
> The investor quality score is 4.0.

---

**👤 You:**
> "Calculate the conversion velocity for 30 total meetings, 10 term sheets, and 5 deals closed."

**🤖 AI Agent:**
> The velocity index is 0.5.


## ❓ FAQ

**Q: How do I calculate the conversion rates for my event?**
You can use the `get_funnel_metrics` tool by providing the number of attendees, scheduled meetings, follow-up meetings, term sheets, and closed deals.

**Q: What determines the investor quality score?**
The score is calculated using `calculate_investor_quality`, which weighs the engagement counts of different investor tiers against the average fund thesis match score.

**Q: Can I measure how fast investors move through my pipeline?**
Yes, the `get_conversion_velocity` tool provides a velocity index that measures the density and speed of your investment funnel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/demo-day-conversion-analytics](https://vinkius.com/ai-agent-connect/demo-day-conversion-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Demo Day Conversion Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `demo-day-conversion-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Demo Day Conversion Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "demo-day-conversion-analytics": {
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
