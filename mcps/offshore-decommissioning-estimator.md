# Offshore Decommissioning Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/offshore-decommissioning-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate structural removal and well P&A costs for offshore energy facilities.

## Description
This MCP server provides specialized tools to estimate the financial requirements of decommissioning offshore energy assets. It calculates structural removal costs based on platform type, size, and water depth, as well as well Plug and Abandon (P&A) costs. Users can determine the total project budget by accounting for different removal methodologies like full or partial removal. Use `estimate_total_decommissioning_cost` to get a complete financial breakdown including both structural and well-related expenditures.


## Available Tools (4)
- **calculate_well_pa_cost**: Calculate the cost to permanently seal the wells (Plug and Abandon)
- **calculate_removal_cost**: Calculate the cost to physically remove the offshore structure
- **estimate_total_decommissioning_cost**: Estimate the total projected budget for the entire decommissioning project
- **get_regional_cost_multipliers**: Get the cost multiplier for a specific geographical region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Offshore Decommissioning Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total decommissioning cost for a Steel Jacket platform with a size of 5000, in 200 meters of water, with 10 wells in the North Sea using full removal?"

**🤖 AI Agent:**
> The total projected decommissioning cost is $45,000,000, which includes $35,000,000 for structural removal and $10,000,000 for well P&A.

---

**👤 You:**
> "How much will it cost to remove a 2000 size FPSO in 500 meters of water in the Gulf of Mexico using partial removal?"

**🤖 AI Agent:**
> The estimated removal cost for the FPSO is $12,500,000 using the partial removal methodology.

---

**👤 You:**
> "Calculate the well P&A cost for 5 wells at a depth of 300 meters in the North Sea."

**🤖 AI Agent:**
> The cost to permanently seal the 5 wells is $4,200,000.


## ❓ FAQ

**Q: What factors influence the decommissioning cost?**
Costs are driven by the platform type, the physical size of the asset, the water depth, the number of wells to be plugged, and the chosen removal methodology.

**Q: How does water depth affect the estimation?**
Increased water depth significantly raises costs due to the need for more complex subsea tooling and specialized vessel requirements.

**Q: Can I estimate the cost for partial removal?**
Yes, you can specify the methodology as 'partial' to estimate costs where only the topsides or a portion of the structure is removed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/offshore-decommissioning-estimator](https://vinkius.com/en/ai-agent-connect/offshore-decommissioning-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Offshore Decommissioning Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `offshore-decommissioning-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Offshore Decommissioning Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "offshore-decommissioning-estimator": {
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
