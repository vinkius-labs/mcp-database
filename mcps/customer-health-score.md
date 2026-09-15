# Customer Health Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/customer-health-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-success](../categories/customer-success.md)

Calculate customer health, churn risk, and expansion opportunities.

## Description
This MCP server provides a comprehensive suite of tools to monitor and predict customer lifecycle outcomes. By aggregating usage frequency, feature adoption, support engagement, NPS, and payment history, it generates a normalized health score. Use `get_customer_health_score` for a high-level overview, `analyze_usage_and_adoption` to measure product stickiness, `evaluate_sentiment_and_support` for satisfaction trends, `assess_financial_health` for payment stability, and `compare_to_segment_benchmarks` to evaluate performance against peer groups.


## Available Tools (5)
- **analyze_usage_and_adoption**: Evaluate how deeply a customer is integrated into the product
- **assess_financial_health**: Determine the stability of the customer relationship based on payment history
- **compare_to_segment_benchmarks**: Compare a customer's metrics against their peer group
- **evaluate_sentiment_and_support**: Assess customer satisfaction and friction
- **get_customer_health_score**: Retrieve the current comprehensive health profile for a specific customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer Health Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current health status of customer CUST-123?"

**🤖 AI Agent:**
> Customer CUST-123 has a health score of 85, which is considered Healthy. The churn risk is Low, and there is a High expansion opportunity.

---

**👤 You:**
> "How is the feature adoption for customer CUST-456?"

**🤖 AI Agent:**
> Customer CUST-456 has a feature adoption percentage of 78% and is currently in a High engagement status.

---

**👤 You:**
> "Is customer CUST-789's sentiment improving?"

**🤖 AI Agent:**
> The sentiment trend for CUST-789 is positive, with an NPS score of 45 and a decreasing volume of support tickets.


## ❓ FAQ

**Q: How is the health score calculated?**
The score is a weighted aggregate of usage frequency, feature adoption, support volume, NPS, and payment reliability, normalized from 0 to 100.

**Q: Can I compare a customer to their specific segment?**
Yes, you can use `compare_to_segment_benchmarks` to see how a customer's metrics deviate from the average of their specific tier, such as Enterprise or SMB.

**Q: What information is needed to check financial stability?**
You only need the `customerId`. You can optionally include a flag to penalize the score for recent late payments using `assess_financial_health`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/customer-health-score](https://vinkius.com/en/ai-agent-connect/customer-health-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer Health Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customer-health-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer Health Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customer-health-score": {
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
