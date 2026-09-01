# Reagent Selection Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reagent-selection-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Identify optimal reagents, reaction conditions, and selectivity for chemical transformations.

## Description
This MCP server provides organic chemists with precise decision support for chemical transformations. Use `find_optimal_reagents` to identify suitable chemical substances, `get_reaction_conditions` to determine temperature and solvent requirements, `check_functional_group_compatibility` to ensure chemoselectivity, and `evaluate_selectivity_profile` to predict regioselectivity and stereoselectivity outcomes.


## Available Tools (4)
- **check_functional_group_compatibility**: Validates whether a proposed reagent will interfere with other groups present in a molecule
- **evaluate_selectivity_profile**: Provides detailed guidance on the spatial or positional outcomes of a reaction
- **find_optimal_reagents**: Identifies the best reagents for a specific transformation based on the starting material and product structure
- **get_reaction_conditions**: Determines the physical environment required for a selected reagent to work


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reagent Selection Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the best reagents to convert Benzene to Nitrobenzene?"

**🤖 AI Agent:**
> The optimal reagent for this nitration is a mixture of concentrated nitric acid and sulfuric acid.

---

**👤 You:**
> "What are the reaction conditions for using PCC in an oxidation?"

**🤖 AI Agent:**
> Pyridinium chlorochromate (PCC) typically requires anhydrous dichloromethane (DCM) as a solvent at room temperature.

---

**👤 You:**
> "Will Lithium Aluminum Hydride react with an ester group?"

**🤖 AI Agent:**
> Yes, Lithium Aluminum Hydride is highly reactive and will reduce esters to primary alcohols.


## ❓ FAQ

**Q: How do I find the best reagents for my reaction?**
You can use the `find_optimal_reagents` tool by providing the starting material and the desired product structure.

**Q: Can I check if a reagent is safe for my specific molecule?**
Yes, use `check_functional_group_compatibility` to validate if a reagent will interfere with other functional groups in your molecule.

**Q: What reaction conditions will be provided?**
The `get_reaction_conditions` tool provides the required temperature range, the ideal solvent system, and the typical reaction duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reagent-selection-guide](https://vinkius.com/ai-agent-connect/reagent-selection-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reagent Selection Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reagent-selection-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reagent Selection Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reagent-selection-guide": {
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
