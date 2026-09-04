# Enterprise Contract Renewal Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-contract-renewal-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate renewal rates, ARR impact, and identify churn risks for enterprise contracts.

## Description
This MCP server provides essential tools for managing enterprise contract lifecycles. It allows AI agents to calculate renewal rates, determine annualized revenue for multi-year agreements using `get_contract_annual_value`, and identify high-risk renewals with `identify_churn_risk`. Additionally, it helps analyze why clients leave through `analyze_churn_drivers` and provides a high-level health summary via `calculate_renewal_metrics`.


## Available Tools (4)
- **identify_churn_risk**: Identifies which upcoming renewals are at highest risk of churn
- **analyze_churn_drivers**: Aggregates and categorizes the reasons why enterprise clients are leaving
- **calculate_renewal_metrics**: Provides a high-level summary of the current renewal health
- **get_contract_annual_value**: Determines the standardized annual value of a contract, accounting for multi-year terms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Contract Renewal Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current renewal health based on these eligible contracts and the ones we've already renewed?"

**🤖 AI Agent:**
> The current renewal rate is 85%, with a total renewal ARR of $1,250,000 from 20 eligible contracts.

---

**👤 You:**
> "Which contracts are at high risk of churning in the next 30 days?"

**🤖 AI Agent:**
> The following contracts are at high risk: CT-992, CT-405, and CT-112.

---

**👤 You:**
> "What is the main reason our enterprise clients are leaving?"

**🤖 AI Agent:**
> The primary churn driver is 'Competitor Switch', accounting for 45% of recent non-renewals.


## ❓ FAQ

**Q: How does the tool handle multi-year contracts?**
The `get_contract_annual_value` tool standardizes revenue by dividing the total contract value by the number of years in the term.

**Q: Can I identify which contracts are most likely to churn?**
Yes, you can use `identify_churn_risk` to categorize upcoming renewals into high, medium, or low risk based on their proximity to the renewal date.

**Q: What metrics are included in the renewal summary?**
The `calculate_renewal_metrics` tool provides the renewal rate percentage, total renewal ARR, total eligible contracts, and total renewed contracts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-contract-renewal-metrics](https://vinkius.com/ai-agent-connect/enterprise-contract-renewal-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Contract Renewal Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-contract-renewal-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Contract Renewal Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-contract-renewal-metrics": {
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
