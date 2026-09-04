# Enterprise Logo Retention Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-logo-retention-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze customer retention rates, tier breakdowns, and churn risks for enterprise segments.

## Description
This MCP server provides specialized analytics for monitoring customer stability. It allows AI agents to calculate the overall logo retention rate using `calculate_logo_retention`, segment retention performance via `analyze_retention_by_tier`, and identify why customers leave with `summarize_churn_reasons`. Additionally, it can forecast future instability using `get_churn_prediction_indicators` to identify high-risk segments based on churn patterns.


## Available Tools (4)
- **get_churn_prediction_indicators**: Identifies emerging churn risks based on tier data and churn events
- **analyze_retention_by_tier**: g., Enterprise, SMB).

Analyzes retention rates across different customer tiers
- **calculate_logo_retention**: Calculates the overall logo retention rate for the period
- **summarize_churn_reasons**: Summarizes the reasons why customers are churning


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Logo Retention Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was our logo retention rate if we started with 100 customers and lost 5?"

**🤖 AI Agent:**
> The logo retention rate is 95%.

---

**👤 You:**
> "Summarize the reasons for churn from these events: [{'reason': 'Price', 'tier': 'Enterprise'}, {'reason': 'Product Gap', 'tier': 'Enterprise'}]"

**🤖 AI Agent:**
> There were 2 total churned customers. The reasons were: Price (1) and Product Gap (1).

---

**👤 You:**
> "Show me the retention breakdown for these tiers: [{'tierName': 'Enterprise', 'tierStartCount': 50, 'tierLostCount': 2}, {'tierName': 'SMB', 'tierStartCount': 100, 'tierLostCount': 10}]"

**🤖 AI Agent:**
> The Enterprise tier has a retention rate of 96%, and the SMB tier has a retention rate of 90%.


## ❓ FAQ

**Q: What is the difference between logo retention and revenue retention?**
Logo retention measures the percentage of unique customer entities maintained, whereas revenue retention measures the percentage of revenue maintained. This tool focuses on the count of unique logos.

**Q: How can I identify which customer segments are most at risk?**
You can use the `get_churn_prediction_indicators` tool to identify segments with high risk scores and their primary churn reasons.

**Q: Can I see retention rates for specific tiers like Enterprise or SMB?**
Yes, the `analyze_retention_by_tier` tool provides a breakdown of retention rates for each customer segment provided in the input.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-logo-retention-analytics](https://vinkius.com/ai-agent-connect/enterprise-logo-retention-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Logo Retention Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-logo-retention-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Logo Retention Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-logo-retention-analytics": {
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
