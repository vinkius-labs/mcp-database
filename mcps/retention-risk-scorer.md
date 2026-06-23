# Retention Risk Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retention-risk-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Predict employee turnover risk and quantify the financial impact of attrition.

## Description
The Retention Risk Scorer is a predictive analytics tool designed to help organizations identify employees at high risk of leaving. By analyzing key human capital metrics such as tenure, promotion history, salary competitiveness, and engagement levels, it provides a normalized turnover risk score (0-100). The server also quantifies the economic burden of vacancies using `estimate_replacement_cost` and offers actionable management strategies through `get_retention_levers`. Use `calculate_risk_score` to evaluate individual profiles and identify primary risk drivers.


## Available Tools (3)
- **estimate_replacement_cost**: Estimate the financial cost of replacing an employee
- **get_retention_levers**: Get recommended management actions to improve retention
- **calculate_risk_score**: Calculate the turnover risk score for an employee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retention Risk Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the turnover risk for an employee with 48 months tenure, 24 months since last promotion, a -15% salary gap, and an engagement score of 60 at the Senior level."

**🤖 AI Agent:**
> The calculated turnover risk score is 72 (High Risk). The primary risk driver identified is the salary gap percentage.

---

**👤 You:**
> "What is the estimated replacement cost for an Executive level employee earning $150,000 per year?"

**🤖 AI Agent:**
> The estimated replacement cost is $375,000. This includes recruitment, onboarding, and lost productivity components.

---

**👤 You:**
> "What actions should I take for an employee with a 85 risk score, -20% salary gap, and 36 months since last promotion?"

**🤖 AI Agent:**
> The prioritized levers are: 1. Review compensation to close the market gap; 2. Evaluate recent performance for potential promotion.


## ❓ FAQ

**Q: How is the turnover risk score calculated?**
The `calculate_risk_score` tool processes tenure, months since last promotion, salary gap percentage, and engagement scores to generate a normalized value between 0 and 100.

**Q: Can I estimate the cost of losing an employee?**
Yes, use the `estimate_replacement_cost` tool by providing the annual salary and seniority level to calculate the projected financial impact.

**Q: Does the tool provide actionable advice?**
Yes, the `get_retention_levers` tool analyzes current risk metrics to suggest prioritized management interventions to mitigate turnover.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retention-risk-scorer](https://vinkius.com/mcp/retention-risk-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retention Risk Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `retention-risk-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retention Risk Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retention-risk-scorer": {
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
