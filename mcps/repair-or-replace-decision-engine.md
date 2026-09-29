# Repair-or-Replace Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-or-replace-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

An automated decision-support engine that evaluates whether to repair an existing asset or replace it with a new one.

## Description
This MCP server provides a suite of analytical tools to help users make informed decisions about asset management. By analyzing item condition, repair quotes, and warranty coverage, the engine determines the most economically and strategically sound path. Use `analyze_repair_viability` to check if a repair is worth the cost, `evaluate_warranty_impact` to calculate effective costs after warranty, and `calculate_decision_plan` to generate a final REPAIR, REPLACE, or NONE recommendation based on your budget and priorities like cost-minimization or longevity.


## Available Tools (4)
- **analyze_repair_viability**: Determines if a repair is physically and economically worth considering for a specific asset
- **calculate_decision_plan**: Generates the final recommendation by weighing all financial and priority-based inputs
- **compare_replacement_options**: Identifies the most suitable replacement item based on availability and budget
- **evaluate_warranty_impact**: Calculates the effective cost of repair by applying warranty coverage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair-or-Replace Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My laptop repair quote is $300, but a new one costs $800. The condition is 'Fair'. Is repair viable?"

**🤖 AI Agent:**
> Yes, the repair is viable as the cost is well within the threshold compared to the replacement cost.

---

**👤 You:**
> "I have a $500 budget. A repair costs $450 and a replacement costs $600. What should I do if I want to minimize cost?"

**🤖 AI Agent:**
> REPAIR. The repair cost of $450 is within your $500 budget and is the cheaper option.

---

**👤 You:**
> "The repair quote is $200, but I have 6 months of warranty left that covers this damage. What is my effective cost?"

**🤖 AI Agent:**
> Your effective repair cost is $0 because the remaining warranty covers the damage.


## ❓ FAQ

**Q: How does the engine decide between repair and replacement?**
The decision is made by weighing the final repair cost against the replacement cost, while strictly adhering to your provided budget limit and strategic priorities like cost-minimization or longevity.

**Q: Can I use this to manage my maintenance budget?**
Yes. By using `calculate_decision_plan`, you can ensure that any recommended action stays within your defined budget limit.

**Q: Does warranty coverage affect the decision?**
Absolutely. The `evaluate_warranty_impact` tool adjusts the initial repair quote to reflect the effective cost after applying any remaining warranty coverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-or-replace-decision-engine](https://vinkius.com/en/ai-agent-connect/repair-or-replace-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair-or-Replace Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-or-replace-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair-or-Replace Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-or-replace-decision-engine": {
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
