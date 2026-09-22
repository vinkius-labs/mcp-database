# Customer Acquisition Cost Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate and analyze marketing spend efficiency and customer acquisition costs.

## Description
This MCP server provides tools to evaluate marketing efficiency by calculating Customer Acquisition Cost (CAC). Use `get_cac_summary` to see total spend and customer counts, `get_cac_by_channel` to identify high-performing platforms, `get_acquisition_efficiency` to check if costs are within business limits, and `get_period_growth_comparison` to track cost trends over time.


## Available Tools (4)
- **get_period_growth_comparison**: Compares the CAC of a target period against a previous period
- **get_acquisition_efficiency**: Compares the CAC against a target threshold
- **get_cac_by_channel**: Breaks down the acquisition cost by specific marketing channels
- **get_cac_summary**: Calculates the overall Customer Acquisition Cost for a specific period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer Acquisition Cost Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was our total CAC and spend for 2023-Q1?"

**🤖 AI Agent:**
> In 2023-Q1, the total marketing spend was $50,000 and we acquired 500 new customers, resulting in a CAC of $100.

---

**👤 You:**
> "Which marketing channels were most efficient in 2023-Jan?"

**🤖 AI Agent:**
> In 2023-Jan, Google Ads had a CAC of $45, while Social Media had a CAC of $65.

---

**👤 You:**
> "Is our acquisition cost within the $50 limit for 2023-Q2?"

**🤖 AI Agent:**
> No, the actual CAC for 2023-Q2 was $55, which exceeds your target limit of $50.


## ❓ FAQ

**Q: How is CAC calculated?**
CAC is calculated by dividing the total marketing spend by the number of new customers acquired during a specific period.

**Q: Can I compare costs between different months?**
Yes, you can use `get_period_growth_comparison` to compare the CAC of a current period against a previous one.

**Q: How do I check if my marketing is efficient?**
You can use `get_acquisition_efficiency` to compare your actual CAC against a target limit you define.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-analytics](https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer Acquisition Cost Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customer-acquisition-cost-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer Acquisition Cost Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customer-acquisition-cost-analytics": {
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
