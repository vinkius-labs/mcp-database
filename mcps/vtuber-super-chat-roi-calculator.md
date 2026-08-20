# VTuber Super Chat ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vtuber-super-chat-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze VTuber stream performance with precise Super Chat revenue, engagement, and whale ratio metrics.

## Description
This MCP server provides deterministic financial and engagement analytics for VTuber streams. It connects AI agents to core streaming metrics, allowing for deep analysis of audience monetization patterns. Use `calculate_stream_metrics` to derive total revenue, conversion rates, and monthly projections. Analyze revenue concentration using `calculate_audience_concentration` to identify the impact of high-value contributors, or use `calculate_engagement_score` to measure the intensity of viewer interaction relative to peak concurrency.


## Available Tools (3)
- **calculate_audience_concentration**: Determines the "whale" ratio to understand how dependent the revenue is on high-value contributors
- **calculate_engagement_score**: Quantifies the "heat" of the stream by measuring how frequently viewers are spending relative to the peak audience size
- **calculate_stream_metrics**: Provides a high-level breakdown of the financial performance and conversion efficiency of a single stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTuber Super Chat ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stream metrics for a stream with 5000 viewers, a duration of 2 hours, and SC tiers of 500 JPY (10 counts) and 5000 JPY (2 counts)."

**🤖 AI Agent:**
> The total revenue for this stream is 15,000 JPY, with a conversion rate of 0.24% and a monthly projection of 450,000 JPY.

---

**👤 You:**
> "What is the whale ratio for these Super Chats: 1000 JPY (50 counts) and 10000 JPY (5 counts)?"

**🤖 AI Agent:**
> The whale ratio is 50.0%, as the top 10% of contributors (5.5 chats) account for 50,000 JPY of the 55,000 JPY total.

---

**👤 You:**
> "Calculate the engagement score for a stream with 100 total Super Chats and a peak concurrency of 500 viewers."

**🤖 AI Agent:**
> The engagement score for this stream is 20.0.


## ❓ FAQ

**Q: How is the monthly projection calculated?**
The monthly projection assumes the current stream's performance metrics are repeated consistently over a standard 30-day period.

**Q: What does the whale ratio represent?**
The whale ratio is the percentage of total revenue contributed by the top 10% of all individual Super Chats, helping identify revenue concentration.

**Q: Can I use this to compare different streams?**
Yes, by using `calculate_engagement_score` and `calculate_stream_metrics`, you can compare the financial efficiency and audience heat across different streaming sessions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vtuber-super-chat-roi-calculator](https://vinkius.com/ai-agent-connect/vtuber-super-chat-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VTuber Super Chat ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vtuber-super-chat-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VTuber Super Chat ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vtuber-super-chat-roi-calculator": {
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
