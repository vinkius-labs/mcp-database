# Newsletter Revenue Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/newsletter-revenue-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Model monthly revenue, profitability, and subscriber retention for newsletter businesses.

## Description
A financial forecasting engine designed for newsletter creators. This MCP server provides tools to model monthly recurring revenue, identify break-even points, and simulate subscriber churn. Use `calculate_monthly_performance` to determine net profit, `calculate_break_even` to find your target audience size, `project_cohort_decay` to visualize subscriber loss over time, and `analyze_revenue_scenarios` to compare different monetization models.


## Available Tools (4)
- **analyze_revenue_scenarios**: Compares different business models
- **calculate_break_even**: Identifies the minimum subscriber count needed to reach a zero-profit state
- **calculate_monthly_performance**: Determines the total revenue and profit for a single specific month
- **project_cohort_decay**: Simulates how a specific group of subscribers loses value over time due to churn


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Newsletter Revenue Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my monthly performance with 5000 subscribers, a 40% open rate, 10% click rate, $10 subscription price, 5% paid conversion, 2 sponsorship slots at $500 each, $200 affiliate commission per click, and $1000 operating cost."

**🤖 AI Agent:**
> Your monthly recurring revenue is $2,500, and your total gross revenue is $3,600. After subtracting the $1,000 operating cost, your net revenue is $2,600.

---

**👤 You:**
> "How many subscribers do I need to break even if my subscription is $5, conversion is 2%, I make $500 from sponsorships, and my costs are $2000?"

**🤖 AI Agent:**
> You need 15,000 subscribers to reach the break-even point.

---

**👤 You:**
> "Project the decay of a cohort of 1000 subscribers with a 5% monthly churn rate over 6 months."

**🤖 AI Agent:**
> After 6 months, you will have approximately 735 subscribers remaining.


## ❓ FAQ

**Q: How do I calculate my monthly profit?**
You can use the `calculate_monthly_performance` tool. Provide your subscriber count, engagement rates, subscription price, and operating costs to see your net revenue.

**Q: Can I simulate how many subscribers I need to cover costs?**
Yes, the `calculate_break_even` tool identifies the minimum subscriber count required to reach a zero-profit state based on your specific revenue streams.

**Q: How does churn affect my long-term revenue?**
You can use `project_cohort_decay` to simulate how a specific group of subscribers loses value over time due to monthly churn rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/newsletter-revenue-planner](https://vinkius.com/en/ai-agent-connect/newsletter-revenue-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Newsletter Revenue Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `newsletter-revenue-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Newsletter Revenue Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "newsletter-revenue-planner": {
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
