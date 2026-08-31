# Limiting Reagent Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/limiting-reagent-yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

A precision stoichiometry engine for determining limiting reactants, theoretical yields, and efficiency metrics.

## Description
This MCP server provides a suite of precision stoichiometry tools for chemical analysis. It allows AI agents to identify limiting reagents using `analyze_reaction_composition`, determine maximum possible product amounts with `calculate_theoretical_yield`, evaluate reaction efficiency via `calculate_actual_and_percent_yield`, and assess mass usage efficiency through `calculate_atom_economy`. It is designed to handle balanced chemical equations and account for side reaction impacts.


## Available Tools (4)
- **analyze_reaction_composition**: Identifies the stoichiometric roles and identifies the limiting reagent from a set of reactants
- **calculate_actual_and_percent_yield**: Calculates how much product was actually obtained and the efficiency of the reaction
- **calculate_atom_economy**: Evaluates the inherent efficiency of the chemical process regarding mass usage
- **calculate_theoretical_yield**: Determines the maximum possible mass or moles of the desired product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Limiting Reagent Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the limiting reagent for the reaction 2H2 + O2 -> 2H2O with 4 moles of H2 and 1 mole of O2."

**🤖 AI Agent:**
> The limiting reagent is O2.

---

**👤 You:**
> "Calculate the theoretical yield of H2O if 2 moles of H2 are used in the reaction 2H2 + O2 -> 2H2O."

**🤖 AI Agent:**
> The theoretical yield is 36.02 grams of H2O.

---

**👤 You:**
> "What is the atom economy for the reaction 2H2 + O2 -> 2H2O?"

**🤖 AI Agent:**
> The atom economy is 100%.


## ❓ FAQ

**Q: How do I identify the limiting reagent?**
You can use the `analyze_reaction_composition` tool by providing the balanced chemical equation and the molar amounts of each reactant.

**Q: Can this tool account for side reactions?**
Yes, the `calculate_actual_and_percent_yield` tool includes an optional parameter to account for reactant loss due to secondary processes.

**Q: What is atom economy?**
Atom economy is a measure of how many atoms from the reactants end up in the desired product, which can be calculated using `calculate_atom_economy`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/limiting-reagent-yield-calculator](https://vinkius.com/ai-agent-connect/limiting-reagent-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Limiting Reagent Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `limiting-reagent-yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Limiting Reagent Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "limiting-reagent-yield-calculator": {
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
