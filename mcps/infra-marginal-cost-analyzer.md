# Infra Marginal Cost Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infra-marginal-cost-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculates unit costs and capacity risks for new customer acquisition.

## Description
This MCP server provides specialized financial analysis for infrastructure scaling. It allows AI agents to determine the unit cost of adding new customers by analyzing incremental capital and operational expenditures against available capacity. Use `calculate_marginal_costs` to find the cost per customer and capacity thresholds, `evaluate_capacity_utilization` to check remaining headroom, `analyze_scale_efficiency` to identify economies of scale, and `capacity_risk_assessment` to evaluate financial risks when approaching capacity limits.


## Available Tools (4)
- **analyze_scale_efficiency**: Analyzes if the system is benefiting from scale or facing diminishing returns
- **calculate_marginal_costs**: Calculates the unit cost of adding specific new customers given current resource constraints
- **capacity_risk_assessment**: Assesses the financial risk of adding customers near the capacity limit
- **evaluate_capacity_utilization**: Evaluates how much of the remaining capacity will be consumed by new customers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infra Marginal Cost Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the marginal cost if I add 50 customers with $10,000 Capex and $5,000 Opex, given 100 units of headroom?"

**🤖 AI Agent:**
> The marginal cost per customer is $300.00, and the capacity threshold is 100 customers.

---

**👤 You:**
> "How much capacity will 20 new customers consume if I have 50 units of headroom left?"

**🤖 AI Agent:**
> The new customers will consume 40% of the available headroom, leaving 30 units remaining.

---

**👤 You:**
> "Is there a high risk in adding 120 customers when I only have 100 units of headroom and $50,000 Capex required?"

**🤖 AI Agent:**
> Yes, the risk level is High because the number of new customers exceeds the available headroom.


## ❓ FAQ

**Q: How do I calculate the cost of adding new customers?**
You can use the `calculate_marginal_costs` tool by providing the incremental Capex, incremental Opex, number of new customers, and current capacity headroom.

**Q: Can this tool help with capacity planning?**
Yes, `evaluate_capacity_utilization` and `capacity_risk_assessment` are designed to help you understand how much headroom remains and the financial risks of exceeding it.

**Q: What is the difference between Capex and Opex in this tool?**
Capex refers to the capital investment for new infrastructure, while Opex refers to the operational expenses required to support the new customer volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infra-marginal-cost-analyzer](https://vinkius.com/ai-agent-connect/infra-marginal-cost-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infra Marginal Cost Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-marginal-cost-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infra Marginal Cost Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-marginal-cost-analyzer": {
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
