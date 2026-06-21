# Blended CAC Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blended-cac-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise Customer Acquisition Cost (CAC) across multiple channels and optimize future marketing spend allocation.

## Description
# Assess Marketing Efficiency with Blended CAC

The core challenge for growing businesses is accurately determining the true cost of acquiring a customer. Relying on single-channel metrics can lead to misallocation of funds, resulting in inefficient spending and stalled growth projections.

Our MCP provides a comprehensive mechanism to bridge this gap by calculating both granular, channel-specific CAC and an overall Blended CAC. It doesn't just report numbers; it prescribes action.

**How the System Works:**
1. **Calculate Foundational Metrics:** The `calculate_cac_metrics` tool takes your spending data (from Paid Search, SEO, etc.) and total customers to determine the basic cost per acquisition for every channel and an overall blended average.
2. **Track Performance Shifts:** Using the `analyze_mom_trend` tool, you can compare current CAC or Total Spend against previous periods. This reveals if your efficiency is improving (negative trend) or worsening (positive trend), allowing for proactive course correction.
3. **Optimize Future Spending:** The system culminates with the `assess_budget_efficiency` tool. It analyzes recent performance alongside industry benchmarks and recommends an optimal percentage split of future marketing dollars. This ensures that every dollar spent maximizes return on investment toward scalable growth.

The result is a clear, actionable financial roadmap. You immediately know which channels to fund more aggressively and where to cut spending for maximum impact.


## Available Tools (3)
- **assess_budget_efficiency**: Returns ranked channels, suggested budget percentages, and natural language recommendations. Provide period data as JSON array of {channelName, spendAmount, calculatedCAC} objects.

Assess budget allocation efficiency and recommend optimal distribution
- **calculate_cac_metrics**: Provide spending data as JSON array of {channelName, spendAmount} objects.

Calculate blended CAC and per-channel CAC for a given period
- **analyze_mom_trend**: Positive means worsening (CAC increased), negative means improving (CAC decreased).

Analyze Month-over-Month trend for CAC or TotalSpend


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blended CAC Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the blended CAC for Q2 2024. We spent $15k on Paid Search, $8k on Paid Social, and $2k on SEO. Total new customers were 300."

**🤖 AI Agent:**
> Using `calculate_cac_metrics` with the provided spending data and customer count of 300, the blended CAC is calculated at $65. The breakdown shows Paid Search contributing $48/customer.

---

**👤 You:**
> "Compare my current CAC to last month's. Last month's CAC was $70, and this month's is $62."

**🤖 AI Agent:**
> Running `analyze_mom_trend` shows a -11.4% change. This negative trend indicates improved efficiency in customer acquisition compared to the previous period.

---

**👤 You:**
> "We are a Technology SaaS company. Given our last quarter's performance (data array) and the industry benchmark, what should my budget split be?"

**🤖 AI Agent:**
> Based on the input data and running `assess_budget_efficiency` for the Technology SaaS sector, we recommend increasing funding for SEO (35% allocation) due to its superior efficiency relative to industry benchmarks.


## ❓ FAQ

**Q: What is the difference between Blended CAC and channel-specific CAC?**
Blended CAC provides a single, overall average cost across all channels. To calculate this, you must use `calculate_cac_metrics`. This tool calculates the total spend divided by total customers, giving you the true company-wide acquisition cost.

**Q: How can I check if my marketing efficiency is getting better or worse over time?**
You should use the `analyze_mom_trend` tool. By comparing CAC or Total Spend between two months, you get a percentage change that immediately tells you if your efficiency trend is positive (negative % change) or negative (positive % change).

**Q: How do I decide where to allocate my budget next month?**
The `assess_budget_efficiency` tool handles this. You provide historical data, and it compares your channels' performance against industry norms to recommend an optimal percentage split for the coming period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blended-cac-calculator](https://vinkius.com/mcp/blended-cac-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blended CAC Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blended-cac-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blended CAC Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blended-cac-calculator": {
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
