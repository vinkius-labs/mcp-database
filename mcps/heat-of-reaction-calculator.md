# Heat of Reaction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/heat-of-reaction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate enthalpy changes using Hess's Law, formation enthalpies, and bond energies.

## Description
This MCP server provides specialized tools for chemical thermodynamics. It allows AI agents to determine the enthalpy change of chemical reactions using two primary methods: standard enthalpies of formation and bond dissociation energies. Users can utilize `calculate_enthalpy_from_formation` to apply Hess's Law directly, or `calculate_enthalpy_from_bond_energy` for gas-phase calculations. Additionally, the server can `generate_enthalpy_diagram` to visualize energy profiles and `identify_reaction_thermodynamics` to classify reactions as exothermic or endothermic.


## Available Tools (4)
- **calculate_enthalpy_from_bond_energy**: Assumes gas phase.

Calculate enthalpy change using bond dissociation energies
- **calculate_enthalpy_from_formation**: Calculate enthalpy change using standard enthalpies of formation
- **generate_enthalpy_diagram**: Generate an energy profile diagram for a reaction
- **identify_reaction_thermodynamics**: Analyze the thermal properties of a reaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heat of Reaction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the enthalpy change for the reaction 2H2 + O2 -> 2H2O if the formation enthalpy of H2O is -285.8 kJ/mol?"

**🤖 AI Agent:**
> The enthalpy change for the reaction is -571.6 kJ/mol, making it an exothermic reaction.

---

**👤 You:**
> "Is the reaction 2H2 + O2 -> 2H2O exothermic or endothermic?"

**🤖 AI Agent:**
> The reaction is exothermic because the enthalpy change is negative.

---

**👤 You:**
> "Calculate the total heat released for 2 moles of a reaction with a delta H of -100 kJ/mol."

**🤖 AI Agent:**
> The total heat released is 200 kJ.


## ❓ FAQ

**Q: How do I calculate enthalpy using formation data?**
You can use the `calculate_enthalpy_from_formation` tool by providing a balanced chemical equation and a JSON object containing the molar enthalpies of formation for each species.

**Q: Does the bond energy calculation work for liquids?**
No, the `calculate_enthalpy_from_bond_energy` tool assumes all reactants and products are in the gaseous phase.

**Q: Can I visualize the energy levels of a reaction?**
Yes, you can use the `generate_enthalpy_diagram` tool to create an energy profile based on the calculated enthalpy change and the enthalpy of reactants and products.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/heat-of-reaction-calculator](https://vinkius.com/ai-agent-connect/heat-of-reaction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heat of Reaction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heat-of-reaction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heat of Reaction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heat-of-reaction-calculator": {
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
