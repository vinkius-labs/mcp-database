# Enterprise Sales Cycle Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-sales-cycle-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [revenue-operations](../categories/revenue-operations.md)

Calculate sales velocity, identify stage bottlenecks, and forecast revenue timelines for enterprise deals.

## Description
This MCP server provides advanced analytics for enterprise sales pipelines. It allows AI agents to calculate the overall speed of the sales process using `analyze_sales_velocity`, compare cycle durations across different deal sizes with `calculate_cycle_by_tier`, and pinpoint friction points using `identify_stage_bottlenecks`. Additionally, it can forecast future revenue by predicting closing dates with `project_revenue_timeline`.


## Available Tools (4)
- **analyze_sales_velocity**: Determines the overall speed and health of the current sales pipeline
- **calculate_cycle_by_tier**: Answers how much longer it takes to close large enterprise deals compared to smaller ones
- **identify_stage_bottlenecks**: Pinpoints which specific stage in the sales process is causing the most significant delays or losses
- **project_revenue_timeline**: Predicts when expected deals will close based on current stage progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Sales Cycle Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current health and speed of my sales pipeline?"

**🤖 AI Agent:**
> The current pipeline velocity is high, with an average cycle of 45 days and an efficiency score of 0.85.

---

**👤 You:**
> "Which stage in our sales process is the biggest bottleneck?"

**🤖 AI Agent:**
> The 'Negotiation' stage is the primary bottleneck due to a high average duration and a low win rate.

---

**👤 You:**
> "When is the $50,000 deal in the 'Proposal' stage expected to close?"

**🤖 AI Agent:**
> The deal is expected to close on October 15th, 2024, with a 75% probability.


## ❓ FAQ

**Q: How can I find where my sales process is stalling?**
You can use the `identify_stage_bottlenecks` tool to find the specific stage causing delays or high loss rates.

**Q: Can I predict when a deal will close?**
Yes, the `project_revenue_timeline` tool calculates expected closing dates and probabilities based on current stage progress.

**Q: Does this tool handle different deal sizes?**
Yes, `calculate_cycle_by_tier` allows you to analyze how sales cycles vary between SMB, Mid-Market, and Enterprise tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-sales-cycle-analyzer](https://vinkius.com/ai-agent-connect/enterprise-sales-cycle-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Sales Cycle Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-sales-cycle-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Sales Cycle Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-sales-cycle-analyzer": {
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
