# Enterprise ARR Productivity Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-arr-productivity-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate sales productivity, ramp-adjusted ARR, and quota attainment metrics.

## Description
This MCP server provides advanced sales productivity analytics. It allows AI agents to calculate baseline ARR per rep using `get_base_productivity`, adjust productivity for new hires via `get_ramp_adjusted_metrics`, and evaluate performance targets with `get_quota_attainment_analysis`. It also enables segment-specific insights through `get_segment_productivity_summary` to ensure fair comparisons across Enterprise, Mid-Market, and SMB tiers.


## Available Tools (4)
- **get_base_productivity**: Calculates the raw, unadjusted ARR generated per salesperson
- **get_quota_attainment_analysis**: Evaluates how well the team is performing against their targets
- **get_segment_productivity_summary**: Aggregates productivity data across different segments or territories
- **get_ramp_adjusted_metrics**: Provides a realistic view of productivity by adjusting for the period where reps are not at full capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise ARR Productivity Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current ARR per rep if we have $10,000,000 ARR and 50 reps?"

**🤖 AI Agent:**
> The current ARR per rep is $200,000.

---

**👤 You:**
> "Calculate the quota attainment for a team with $8,000,000 ARR against a $10,000,000 quota and 40 reps."

**🤖 AI Agent:**
> The overall attainment is 80%, the average quota per rep is $250,000, and the capacity gap is $2,000,000.

---

**👤 You:**
> "Adjust our productivity for 10,000,000 ARR, 50 reps, a 6 month ramp, and 5 reps in their first 3 months."

**🤖 AI Agent:**
> The ramp-adjusted ARR per rep is $217,391.30 based on an effective capacity of 46 reps.


## ❓ FAQ

**Q: How does the tool account for new sales hires?**
The `get_ramp_adjusted_metrics` tool accounts for new hires by adjusting the effective headcount based on the provided tenure distribution and ramp months.

**Q: Can I analyze specific market segments?**
Yes, you can use `get_base_productivity` with a segment ID or `get_segment_productivity_summary` to analyze performance across different tiers like Enterprise or SMB.

**Q: What is the capacity gap?**
The capacity gap is the difference between the total assigned quota and the actual ARR achieved, which can be found using `get_quota_attainment_analysis`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-arr-productivity-analyzer](https://vinkius.com/ai-agent-connect/enterprise-arr-productivity-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise ARR Productivity Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-arr-productivity-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise ARR Productivity Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-arr-productivity-analyzer": {
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
