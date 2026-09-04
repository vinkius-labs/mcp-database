# Enterprise Health Score Calculation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-health-score-calculation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-success](../categories/customer-success.md)

Calculate multi-dimensional customer health scores, trends, and risk indicators.

## Description
This MCP server provides a specialized engine for calculating multi-dimensional customer health scores. It analyzes product usage, engagement metrics, support tickets, NPS, payment history, and stakeholder relationships to provide a comprehensive view of customer stability. Use `get_customer_health_score` to obtain the absolute score and trend, `analyze_usage_risk` to identify engagement-based risks, `get_relationship_and_sentiment_health` for qualitative relationship data, and `get_financial_and_support_stability` for operational health assessments.


## Available Tools (4)
- **analyze_usage_risk**: Identifies specific risks stemming solely from product usage and engagement patterns
- **get_customer_health_score**: Calculates the current absolute health score and trend for a specific customer
- **get_financial_and_support_stability**: Assesses the operational health of the customer based on payment behavior and support interactions
- **get_relationship_and_sentiment_health**: Evaluates the qualitative aspects of the customer relationship, including NPS and stakeholder strength


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Health Score Calculation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current health score and trend for customer CUST-123?"

**🤖 AI Agent:**
> Customer CUST-123 has a health score of 85 with an improving trend.

---

**👤 You:**
> "Are there any usage risks for customer CUST-456?"

**🤖 AI Agent:**
> Customer CUST-456 shows a declining engagement score due to a drop in session frequency.

---

**👤 You:**
> "Check the relationship health for customer CUST-789."

**🤖 AI Agent:**
> Customer CUST-789 has a high stakeholder strength and a positive NPS status.


## ❓ FAQ

**Q: How is the health score calculated?**
The score is a weighted calculation that adapts based on the customer's segment (SMB, Mid-Market, or Enterprise) and specific use case, incorporating usage, sentiment, and stability metrics.

**Q: Can I analyze specific usage risks?**
Yes, you can use the `analyze_usage_risk` tool to identify specific risks stemming from product usage and engagement patterns.

**Q: Does the score account for financial stability?**
Yes, the `get_financial_and_support_stability` tool assesses operational health by looking at payment behavior and support interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-health-score-calculation](https://vinkius.com/ai-agent-connect/enterprise-health-score-calculation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Health Score Calculation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-health-score-calculation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Health Score Calculation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-health-score-calculation": {
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
