# Mine Closure Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mine-closure-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total financial liability for mine closure, including remediation and monitoring.

## Description
This MCP server provides specialized tools for quantifying the total financial liability of mine closure. It allows users to calculate direct remediation costs using `calculate_activity_costs`, project long-term environmental expenses with `estimate_monitoring_costs`, aggregate all costs via `calculate_total_liability`, and determine regulatory bonding requirements through `determine_financial_assurance`. It is designed to help mining operators and regulators manage financial assurance and post-closure monitoring obligations accurately.


## Available Tools (4)
- **calculate_activity_costs**: Determine the direct cost of specific remediation tasks based on the physical footprint and chosen activities
- **calculate_total_liability**: Aggregate all closure-related costs into a single total liability figure
- **determine_financial_assurance**: Calculate the final amount required to satisfy regulatory guarantee/bonding requirements
- **estimate_monitoring_costs**: Calculate the long-term environmental monitoring expenses following the completion of physical works


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Closure Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the direct cost for 50 hectares of disturbance with earthmoving at $5000/ha and seeding at $2000/ha."

**🤖 AI Agent:**
> The total direct cost for the specified activities is $350,000.

---

**👤 You:**
> "What is the total monitoring cost for an annual expense of $10,000 over 10 years with 2% inflation?"

**🤖 AI Agent:**
> The total monitoring cost over 10 years with a 2% annual inflation rate is $109,497.21.

---

**👤 You:**
> "Calculate the total liability if direct costs are $500,000, monitoring costs are $100,000, and I want a 10% contingency."

**🤖 AI Agent:**
> The total liability, including a $60,000 contingency, is $660,000.


## ❓ FAQ

**Q: How do I calculate the cost of specific reclamation tasks?**
You can use the `calculate_activity_costs` tool by providing the total disturbance area, a list of activities, and a JSON mapping of unit rates per hectare.

**Q: Can I account for inflation in monitoring costs?**
Yes, the `estimate_monitoring_costs` tool includes an optional inflation rate parameter to account for annual increases over the monitoring duration.

**Q: How is the final regulatory bond amount determined?**
The `determine_financial_assurance` tool calculates the required amount by applying a regulatory multiplier to the total liability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mine-closure-cost-estimator](https://vinkius.com/ai-agent-connect/mine-closure-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Closure Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-closure-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Closure Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-closure-cost-estimator": {
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
