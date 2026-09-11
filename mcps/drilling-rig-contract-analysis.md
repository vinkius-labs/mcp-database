# Drilling Rig Contract Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/drilling-rig-contract-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-management](../categories/risk-management.md)

Economic evaluation and risk assessment for drilling rig procurement strategies.

## Description
This MCP server provides specialized tools for oil and gas operators to evaluate the financial impact of drilling rig procurement. It enables precise calculation of total well costs using `get_total_well_cost`, quantifies financial exposure through `evaluate_duration_risk`, and compares long-term term contracts against spot market volatility with `compare_contract_strategies`. Additionally, it assesses market supply and demand via `analyze_rig_availability` to determine if rig procurement is secure or critical.


## Available Tools (4)
- **analyze_rig_availability**: Assesses the feasibility of a drilling plan based on current market supply and demand
- **compare_contract_strategies**: Determines whether a long-term Term contract or a short-term Spot market approach is more economically sound
- **evaluate_duration_risk**: Quantifies the financial exposure if the well program takes longer than expected
- **get_total_well_cost**: Calculates the complete financial requirement for a single rig deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drilling Rig Contract Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a 30-day well with a $50,000 day rate and $200,000 mobilization fee?"

**🤖 AI Agent:**
> The total well cost is $1,700,000, with an effective daily rate of $56,666.67.

---

**👤 You:**
> "If my planned duration is 40 days and I expect a 5-day delay at a $60,000 day rate, what is my risk?"

**🤖 AI Agent:**
> The delay cost is $300,000, representing a 12.5% risk relative to the original planned cost.

---

**👤 You:**
> "Is it better to use a term contract at $55,000/day or a spot market at $60,000/day for a 50-day operation with a volatility index of 0.1?"

**🤖 AI Agent:**
> The recommended strategy is TERM, as the adjusted spot cost is higher due to market volatility.


## ❓ FAQ

**Q: How do I calculate the total cost of a rig deployment?**
You can use the `get_total_well_cost` tool by providing the planned duration, the daily rate, and the mobilization cost.

**Q: Can this tool help me decide between a term contract and the spot market?**
Yes, the `compare_contract_strategies` tool compares term and spot rates while accounting for market volatility to recommend the most economical approach.

**Q: How is duration risk measured?**
The `evaluate_duration_risk` tool calculates the additional cost incurred from delays and the resulting risk percentage relative to the original plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/drilling-rig-contract-analysis](https://vinkius.com/ai-agent-connect/drilling-rig-contract-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drilling Rig Contract Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drilling-rig-contract-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drilling Rig Contract Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drilling-rig-contract-analysis": {
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
