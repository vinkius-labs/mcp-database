# Monthly Recurring Revenue (MRR) Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/monthly-recurring-revenue-mrr-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate MRR growth, churn analysis, and future revenue projections.

## Description
This MCP server provides essential financial intelligence for subscription-based businesses. It allows AI agents to perform deep analysis of revenue health using tools like `get_mrr_movement_summary` to track net growth, `get_mrr_churn_analysis` to evaluate retention, and `get_mrr_projection` to forecast future revenue based on growth rates and seasonality. It also includes `get_cohort_health_metrics` to monitor how specific customer groups perform over time.


## Available Tools (4)
- **get_cohort_health_metrics**: Evaluates how different customer groups (cohorts) are performing over time
- **get_mrr_churn_analysis**: Provides a deep dive into the health of the customer base by isolating churn impacts
- **get_mrr_movement_summary**: Calculates the immediate changes in MRR for a specific period to determine net growth
- **get_mrr_projection**: Predicts future MRR based on growth rates and historical patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monthly Recurring Revenue (MRR) Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my net new MRR if I started with $10,000, gained $2,000 in new MRR, had $500 in expansion, and lost $300 to churn."

**🤖 AI Agent:**
> Your net new MRR is $2,200, resulting in a total MRR of $12,200 after movement.

---

**👤 You:**
> "Project my MRR for the next 3 months if I have $50,000 current MRR and a 5% monthly growth rate."

**🤖 AI Agent:**
> Your projected MRR after 3 months will be $57,881.25.

---

**👤 You:**
> "What is my churn rate if I have $10,000 MRR and lost $500 to cancellations and $200 to downgrades?"

**🤖 AI Agent:**
> Your churn rate is 7%.


## ❓ FAQ

**Q: How can I predict my revenue for the next six months?**
You can use the `get_mrr_projection` tool. Provide your current MRR, expected monthly growth rate, and set the projection months to 6.

**Q: What is the difference between churn and contraction?**
Churn refers to customers leaving entirely, while contraction refers to existing customers downgrading their plans. Both are analyzed using `get_mrr_churn_analysis`.

**Q: Can I analyze specific customer cohorts?**
Yes, the `get_cohort_health_metrics` tool allows you to evaluate the performance and lifetime value of specific customer groups based on their age and churn rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/monthly-recurring-revenue-mrr-analyzer](https://vinkius.com/en/ai-agent-connect/monthly-recurring-revenue-mrr-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monthly Recurring Revenue (MRR) Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `monthly-recurring-revenue-mrr-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monthly Recurring Revenue (MRR) Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monthly-recurring-revenue-mrr-analyzer": {
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
