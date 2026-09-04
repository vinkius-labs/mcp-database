# Enterprise NRR Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-nrr-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Net Revenue Retention (NRR) and expansion potential for enterprise accounts.

## Description
This MCP server provides specialized tools for analyzing SaaS revenue health. It allows AI agents to calculate NRR percentage, identify negative churn status, and evaluate untapped revenue capacity. Use `calculate_nrr_metrics` to get a full health overview, `evaluate_expansion_potential` to find upsell opportunities, `analyze_churn_composition` to identify loss drivers, and `get_cohort_health_summary` for high-level account health scores.


## Available Tools (4)
- **analyze_churn_composition**: Breaks down the components of revenue loss to identify if the primary issue is customer attrition or service downgrades
- **calculate_nrr_metrics**: Provides a comprehensive overview of revenue retention health for a specific period or cohort
- **evaluate_expansion_potential**: Estimates the untapped revenue capacity within the current customer base
- **get_cohort_health_summary**: Generates a high-level summary of the relationship between account volume and revenue retention


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise NRR Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NRR metrics for a cohort with $100,000 starting ARR, $20,000 expansion, $5,000 contraction, and $5,000 churn across 50 accounts."

**🤖 AI Agent:**
> The NRR for this cohort is 110.0%, indicating a healthy expansion that offsets all losses.

---

**👤 You:**
> "What is the expansion potential for an account with $50,000 ARR, 80 max seats, 50 current seats, and $1,000 average revenue per seat?"

**🤖 AI Agent:**
> The expansion gap is $30,000, with a seat utilization of 62.5%.

---

**👤 You:**
> "Analyze the churn for a period where we lost $10,000 to churn and $2,000 to contraction."

**🤖 AI Agent:**
> The primary loss driver is Churn, which accounts for 83.3% of the total revenue loss.


## ❓ FAQ

**Q: How is NRR calculated?**
NRR is calculated by taking the starting ARR, adding expansion revenue, and subtracting contraction and churned revenue, then dividing the result by the starting ARR.

**Q: What is negative churn?**
Negative churn occurs when expansion revenue from existing customers exceeds the total revenue lost from contractions and churn.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-nrr-analytics](https://vinkius.com/ai-agent-connect/enterprise-nrr-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise NRR Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-nrr-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise NRR Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-nrr-analytics": {
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
