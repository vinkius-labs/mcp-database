# Sales Quota Attainment Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sales-quota-attainment-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Track sales progress, evaluate performance against targets, and project required daily sales velocity.

## Description
This MCP server provides a specialized calculation engine for sales teams to monitor their progress toward revenue targets. It allows AI agents to calculate real-time attainment metrics, evaluate pipeline health using historical conversion rates, and determine the exact daily revenue needed to close the gap to quota. Use `calculate_attainment_metrics` for a full performance snapshot, `analyze_pipeline_health` to check if your current pipeline can meet targets, or `get_attainment_summary` for a quick progress check.


## Available Tools (4)
- **analyze_pipeline_health**: Evaluates if the current pipeline is sufficient to meet the quota based on historical conversion trends
- **calculate_attainment_metrics**: Provides a comprehensive snapshot of current performance and the path to completion
- **get_attainment_summary**: Returns a simplified high-level summary of the attainment progress
- **validate_sales_inputs**: Validates the integrity of sales data before performing heavy calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sales Quota Attainment Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a quota of $100,000, I've closed $40,000, my pipeline is $50,000, I have 10 days left, and my historical close rate is 20%. What is my current status?"

**🤖 AI Agent:**
> Your current attainment is 40%. You have a gap of $60,000 to reach your quota. To hit your target, you need a required daily rate of $6,000 for the remaining 10 days.

---

**👤 You:**
> "Give me a quick summary: Quota is $50,000 and I have closed $45,000."

**🤖 AI Agent:**
> You have reached 90% of your target, with $5,000 remaining to reach your $50,000 quota.

---

**👤 You:**
> "Is my pipeline healthy? Quota $200,000, closed $50,000, pipeline $150,000, historical close rate 0.5."

**🤖 AI Agent:**
> Your weighted pipeline is $75,000. Since you still need $150,000 to reach your quota, your sufficiency ratio is 0.5, indicating your current pipeline is not sufficient to meet the target.


## ❓ FAQ

**Q: How do I calculate my daily sales requirement?**
You can use the `calculate_attainment_metrics` tool. It takes your quota, closed revenue, pipeline value, days remaining, and historical close rate to provide the exact `requiredDailyRate` needed to hit your target.

**Q: Can this tool help me predict if I will hit my target?**
Yes. By using `analyze_pipeline_health`, the engine compares your weighted pipeline against your remaining quota to provide a sufficiency ratio and a projected attainment percentage.

**Q: What inputs are required for the calculations?**
Most tools require the total quota, closed revenue, and pipeline value. For advanced metrics, you will also need the number of days remaining and your historical close rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sales-quota-attainment-engine](https://vinkius.com/en/ai-agent-connect/sales-quota-attainment-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sales Quota Attainment Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sales-quota-attainment-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sales Quota Attainment Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sales-quota-attainment-engine": {
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
