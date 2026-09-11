# Unitization Allocations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/unitization-allocations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates unitization equity, cost allocations, and revenue distributions.

## Description
This MCP server provides specialized tools for the oil and gas industry to manage unitization processes. It connects AI agents to core calculation engines for determining ownership interests and financial distributions. Use `get_equity_determination` to calculate ownership based on tract reserves, `calculate_financial_distributions` to split revenue and costs, `apply_redetermination` to update equity when new geological data arrives, and `get_historical_adjustments` to correct past payments.


## Available Tools (4)
- **apply_redetermination**: Updates the unit's ownership structure based on new geological data
- **calculate_financial_distributions**: Determines how much money should be paid to or charged to each party based on recent activity
- **get_equity_determination**: Calculates the current ownership interest for all parties involved in the unit
- **get_historical_adjustments**: Identifies the necessary corrections for past distributions due to changes in equity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unitization Allocations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the equity for two parties where Party A has 600 units of reserves and Party B has 400 units."

**🤖 AI Agent:**
> Party A has 60% equity and Party B has 40% equity.

---

**👤 You:**
> "If total revenue is $1,000,000 and costs are $200,000, what is the net amount for a party with 50% equity?"

**🤖 AI Agent:**
> The net amount for the party is $400,000.

---

**👤 You:**
> "What happens if we use `apply_redetermination` with new reserve volumes?"

**🤖 AI Agent:**
> The tool will calculate the new equity percentages and provide an adjustment factor based on the change in total reserves.


## ❓ FAQ

**Q: How is equity determined?**
Equity is determined by dividing a party's specific reserve volume by the total reserves of the entire unit using the `get_equity_determination` tool.

**Q: Can I adjust for new geological data?**
Yes, you can use `apply_redetermination` to update the unit's ownership structure based on new reserve volumes.

**Q: How are historical errors corrected?**
You can identify necessary corrections for past distributions using the `get_historical_adjustments` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/unitization-allocations](https://vinkius.com/en/ai-agent-connect/unitization-allocations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unitization Allocations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unitization-allocations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unitization Allocations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unitization-allocations": {
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
