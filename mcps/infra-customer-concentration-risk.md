# Infra Customer Concentration Risk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infra-customer-concentration-risk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantifies financial vulnerability by analyzing revenue distribution and customer stability.

## Description
This MCP server provides a specialized risk assessment engine for infrastructure businesses. It quantifies financial vulnerability by analyzing how revenue is distributed across a customer base. Using tools like `calculate_hhi` and `evaluate_risk_score`, it calculates the Herfindahl-Hirschman Index (HHI), top 10 customer concentration, and a holistic risk score that accounts for contract duration and switching costs. It helps identify 'Whale' accounts and assess the impact of potential customer churn.


## Available Tools (4)
- **analyze_revenue_distribution**: Provides a detailed breakdown of how revenue is distributed across the customer base
- **calculate_hhi**: Quantifies the level of revenue concentration using the HHI method
- **calculate_top_ten_concentration**: Determines the total revenue exposure concentrated within the largest ten clients
- **evaluate_risk_score**: Generates a holistic risk score by adjusting concentration metrics with contract stability and switching costs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infra Customer Concentration Risk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the HHI for these revenue shares: 40, 30, 20, 10."

**🤖 AI Agent:**
> The calculated HHI index is 3000, which indicates a High concentration level.

---

**👤 You:**
> "What is the concentration of the top 10 customers if the shares are 50, 20, 10, 5, 5, 2, 2, 2, 2, 2?"

**🤖 AI Agent:**
> The top 10 concentration is 100%.

---

**👤 You:**
> "Evaluate the risk score for an HHI of 2500, top 10 concentration of 80%, average contract duration of 3 years, and switching cost of 7."

**🤖 AI Agent:**
> The risk score is 65, which falls into the Warning category.


## ❓ FAQ

**Q: What is the HHI index?**
The Herfindahl-Hirschman Index (HHI) is a statistical measure of revenue concentration. You can calculate it using the `calculate_hhi` tool.

**Q: How does contract duration affect the risk score?**
Longer contract durations act as a buffer, reducing the overall risk score when processed through `evaluate_risk_score`.

**Q: Can I see a breakdown of my customer tiers?**
Yes, the `analyze_revenue_distribution` tool provides a tier breakdown including Whale, Key Accounts, and Fragmented customers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infra-customer-concentration-risk](https://vinkius.com/ai-agent-connect/infra-customer-concentration-risk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infra Customer Concentration Risk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-customer-concentration-risk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infra Customer Concentration Risk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-customer-concentration-risk": {
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
