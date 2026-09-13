# Oil Supply Chain Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/oil-supply-chain-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimize crude oil routing, inventory levels, and quality compliance across the supply chain.

## Description
This MCP server provides specialized tools to manage the complex logistics of moving crude oil from production sites to refineries. It calculates the most cost-effective paths using `get_optimal_routing`, determines necessary storage levels with `calculate_inventory_targets`, ensures chemical requirements are met via `evaluate_quality_compliance`, and validates infrastructure limits with `simulate_transportation_capacity`.


## Available Tools (4)
- **calculate_inventory_targets**: Determines the necessary storage levels at production and refinery nodes
- **evaluate_quality_compliance**: Checks if a proposed supply plan meets the chemical requirements of the refineries
- **get_optimal_routing**: Finds the most cost-effective paths to move crude from production to refineries
- **simulate_transportation_capacity**: Validates if the physical infrastructure can handle the proposed optimal routing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oil Supply Chain Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best way to move oil from production site A to refinery B."

**🤖 AI Agent:**
> The optimal route is via pipeline with a total cost of $45,000 for 5,000 barrels.

---

**👤 You:**
> "Is the crude from site Alpha compliant with Refinery X's constraints?"

**🤖 AI Agent:**
> Yes, the crude quality profile meets all the required chemical parameters for Refinery X.

---

**👤 You:**
> "What are the target inventory levels for the refinery nodes?"

**🤖 AI Agent:**
> The target stock for Refinery Node 1 is 12,000 barrels to maintain the safety buffer.


## ❓ FAQ

**Q: How does the tool handle crude quality constraints?**
The `evaluate_quality_compliance` tool checks if the chemical properties of a crude source fall within the specific input windows required by a refinery.

**Q: Can I check if my pipelines can handle the planned volume?**
Yes, you can use `simulate_transportation_capacity` to validate if the physical infrastructure can handle the proposed routing and identify potential bottlenecks.

**Q: Does this tool calculate storage needs?**
Yes, `calculate_inventory_targets` determines the necessary storage levels at both production and refinery nodes to ensure continuous supply.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/oil-supply-chain-optimizer](https://vinkius.com/en/ai-agent-connect/oil-supply-chain-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oil Supply Chain Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oil-supply-chain-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oil Supply Chain Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oil-supply-chain-optimizer": {
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
