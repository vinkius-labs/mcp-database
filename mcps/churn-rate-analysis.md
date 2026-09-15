# Churn Rate Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/churn-rate-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate customer churn, net growth, revenue impact, and churn composition.

## Description
This MCP server provides a suite of analytical tools to monitor customer retention and revenue health. Use `get_customer_churn_metrics` to find the basic churn rate, `get_net_churn_status` to see if your user base is growing or shrinking, `get_revenue_churn_impact` to measure financial loss, and `get_churn_composition` to distinguish between voluntary and involuntary departures.


## Available Tools (4)
- **get_churn_composition**: Breaks down the reasons for customer loss to distinguish between intentional and unintentional departures
- **get_customer_churn_metrics**: Calculates the basic percentage of customers lost during a period
- **get_net_churn_status**: Determines if the customer base is growing or shrinking by factoring in new acquisitions
- **get_revenue_churn_impact**: Analyzes the financial impact of customer losses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Churn Rate Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the churn rate if I started with 100 customers and lost 5 this month?"

**🤖 AI Agent:**
> The customer churn rate for this period is 5%.

---

**👤 You:**
> "Is my business growing? I had 500 customers, lost 20, but gained 50 new ones."

**🤖 AI Agent:**
> Your customer base is Growing, with a net churn rate of -6%.

---

**👤 You:**
> "Calculate the revenue impact: we had $10,000 MRR and lost $1,000 due to cancellations."

**🤖 AI Agent:**
> The revenue churn rate is 10% and the revenue retention rate is 90%.


## ❓ FAQ

**Q: How do I calculate the basic churn rate?**
You can use the `get_customer_churn_metrics` tool by providing the number of customers at the start of the period and the number of customers lost.

**Q: Can I distinguish between voluntary and involuntary churn?**
Yes, the `get_churn_composition` tool allows you to break down losses into voluntary and involuntary percentages.

**Q: How does this tool help with revenue analysis?**
The `get_revenue_churn_impact` tool calculates both the revenue churn rate and the revenue retention rate based on your starting MRR.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/churn-rate-analysis](https://vinkius.com/en/ai-agent-connect/churn-rate-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Churn Rate Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `churn-rate-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Churn Rate Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "churn-rate-analysis": {
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
