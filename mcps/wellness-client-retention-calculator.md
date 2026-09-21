# Wellness Client Retention Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-client-retention-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Calculate retention rates, churn, and client lifetime value for wellness businesses.

## Description
This MCP server provides essential analytics for wellness businesses to monitor client loyalty and revenue stability. Use `get_retention_metrics` to calculate core retention and churn percentages, `calculate_client_lifetime_value` to project long-term revenue per client, and `generate_retention_strategies` to receive actionable advice for improving loyalty. You can also use `get_business_health_summary` to get a high-level overview of your business state.


## Available Tools (4)
- **calculate_client_lifetime_value**: Determines the total projected revenue from a single client
- **generate_retention_strategies**: Provides qualitative business advice to improve client loyalty based on current performance
- **get_business_health_summary**: Provides a high-level overview of the business state by combining multiple metrics
- **get_retention_metrics**: Calculates the core retention and churn percentages for a wellness business


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Client Retention Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my retention and churn rates if I had 50 new clients, 80 returning clients, and 20 lost clients?"

**🤖 AI Agent:**
> Your retention rate is 80% and your churn rate is 20%.

---

**👤 You:**
> "Calculate the lifetime value for a client if the average revenue is $100 and the churn rate is 0.1."

**🤖 AI Agent:**
> The client lifetime value is $1,000.

---

**👤 You:**
> "Give me a health summary for a business with 90% retention, 10% churn, and $5,000 lifetime value."

**🤖 AI Agent:**
> Status: Stable. Your business shows strong client loyalty and healthy revenue projections.


## ❓ FAQ

**Q: How do I calculate my retention rate?**
You can use the `get_retention_metrics` tool by providing the number of new clients, returning clients, and lost clients for your chosen period.

**Q: What is Client Lifetime Value (CLV)?**
CLV is the total projected revenue a single client will generate. Use `calculate_client_lifetime_value` to determine this based on your average revenue per client and current churn rate.

**Q: Can this tool help improve my business?**
Yes. By using `generate_retention_strategies`, you receive specific, actionable recommendations to improve client loyalty based on your current retention performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-client-retention-calculator](https://vinkius.com/en/ai-agent-connect/wellness-client-retention-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Client Retention Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-client-retention-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Client Retention Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-client-retention-calculator": {
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
