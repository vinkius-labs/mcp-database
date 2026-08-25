# Dairy Somatic Cell Score Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dairy-somatic-cell-score-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate bulk tank somatic cell count (BTSCC) contributions and quantify mastitis economic impact.

## Description
This MCP server provides specialized analytical tools for dairy producers to monitor herd health and profitability. It allows for the calculation of volume-weighted bulk tank somatic cell count (BTSCC) using `get_weighted_btscs`. Producers can estimate financial losses from mastitis using `calculate_economic_impact`, determine if individual cows should be removed from the herd via `evaluate_culling_status`, and model potential infection spread with `predict_outbreak_scenario`.


## Available Tools (4)
- **get_weighted_btscs**: Calculates the total somatic cell contribution of the whole herd to the bulk tank
- **predict_outbreak_scenario**: Models how an infection might spread through the herd based on current infection levels
- **evaluate_culling_status**: Determines if a cow has exceeded the threshold for economic viability
- **calculate_economic_impact**: Estimates the total financial loss for a specific cow or a herd due to mastitis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dairy Somatic Cell Score Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the weighted BTSCC for a herd where Cow A has an SCC score of 250 and produces 30kg of milk, and Cow B has an SCC score of 400 and produces 20kg of milk."

**🤖 AI Agent:**
> The weighted BTSCC for the herd is 300.

---

**👤 You:**
> "What is the economic impact for a cow with an SCC score of 500, producing 40kg of milk, with a milk price of 0.40 and a penalty of 0.05 per unit of SCC?"

**🤖 AI Agent:**
> The total economic loss for this cow is 2.00.

---

**👤 You:**
> "Predict the outbreak risk if there are 5 infected cows in a herd of 100 with a transmission factor of 1.5."

**🤖 AI Agent:**
> The predicted number of infected cows is 7, and the risk level is low.


## ❓ FAQ

**Q: How is the bulk tank SCC calculated?**
The `get_weighted_btscs` tool calculates a volume-weighted average, ensuring that cows producing more milk have a proportional impact on the total bulk tank score.

**Q: Can I estimate the cost of mastitis in my herd?**
Yes, by using `calculate_economic_impact`, you can estimate production losses and quality penalties based on current SCC levels and milk prices.

**Q: How do I know if a cow should be culled?**
The `evaluate_culling_status` tool compares a cow's current SCC score against your defined economic threshold to recommend if culling is necessary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dairy-somatic-cell-score-analyzer](https://vinkius.com/ai-agent-connect/dairy-somatic-cell-score-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dairy Somatic Cell Score Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dairy-somatic-cell-score-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dairy Somatic Cell Score Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dairy-somatic-cell-score-analyzer": {
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
