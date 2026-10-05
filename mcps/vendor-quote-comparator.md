# Vendor Quote Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vendor-quote-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Compare supplier quotes by unit price, lead time, and risk.

## Description
This MCP server provides tools to evaluate and compare supplier quotes across multiple dimensions. Use `compare_quotes` to calculate landed costs, `evaluate_risk_profile` to rank vendors by stability, `calculate_cash_flow_impact` to analyze liquidity, and `find_optimal_vendor` to identify the best supplier using weighted objectives.


## Available Tools (4)
- **calculate_cash_flow_impact**: 
- **compare_quotes**: 
- **evaluate_risk_profile**: 
- **find_optimal_vendor**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vendor Quote Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these three quotes for 500 units: Vendor A (Price: 10, MOQ: 100, Freight: 50, Lead: 5, Defect: 0.01), Vendor B (Price: 9, MOQ: 500, Freight: 200, Lead: 10, Defect: 0.02), and Vendor C (Price: 12, MOQ: 50, Freight: 20, Lead: 2, Defect: 0.005)."

**🤖 AI Agent:**
> Vendor A has the lowest landed cost per unit at $10.10, while Vendor C offers the fastest lead time of 2 days.

---

**👤 You:**
> "Which vendor is best if I prioritize quality above all else for 1000 units?"

**🤖 AI Agent:**
> Vendor C is the optimal choice due to its extremely low defect rate of 0.005.

---

**👤 You:**
> "Show me the cash flow impact for these quotes with a target of 200 units."

**🤖 AI Agent:**
> Vendor A requires an outflow of $2,050, while Vendor B requires $1,100 due to the MOQ requirement.


## ❓ FAQ

**Q: How do I compare multiple vendors at once?**
You can use the `compare_quotes` tool by providing an array of quote objects and your target quantity.

**Q: Can I prioritize speed over cost?**
Yes, use the `evaluate_risk_profile` tool and set the priority metric to 'speed' to rank vendors based on lead times.

**Q: How is the best vendor determined?**
The `find_optimal_vendor` tool identifies the best supplier by applying weights to cost, speed, and quality metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vendor-quote-comparator](https://vinkius.com/en/ai-agent-connect/vendor-quote-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vendor Quote Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vendor-quote-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vendor Quote Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vendor-quote-comparator": {
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
