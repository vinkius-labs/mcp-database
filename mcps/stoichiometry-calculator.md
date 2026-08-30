# Stoichiometry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/stoichiometry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Perform precise chemical stoichiometry calculations including limiting reagents and theoretical yields.

## Description
This MCP server provides a precision calculation engine for chemical stoichiometry. It allows AI agents to analyze balanced chemical equations to determine the limiting reagent, calculate the amount of excess reagents remaining, and find the theoretical yield of specific products. Users can also evaluate reaction efficiency by comparing actual yields to theoretical limits using the `calculate_percent_yield` tool. It is designed to handle molar mass calculations and stoichiometric ratios automatically.


## Available Tools (4)
- **calculate_percent_yield**: Evaluates the efficiency of a reaction by comparing actual results to theoretical limits
- **calculate_reaction_composition**: Identifies the limiting reagent and the amount of excess reagent remaining
- **calculate_theoretical_yield**: Determines the maximum possible mass of a specific product
- **validate_equation_and_masses**: A utility to verify the chemical validity of an equation and the presence of all necessary mass data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stoichiometry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the limiting reagent for the reaction 2H2 + O2 -> 2H2O with 4g of H2 and 32g of O2."

**🤖 AI Agent:**
> The limiting reagent is H2.

---

**👤 You:**
> "What is the theoretical yield of H2O if I react 4g of H2 and 32g of O2 in the reaction 2H2 + O2 -> 2H2O?"

**🤖 AI Agent:**
> The theoretical yield of H2O is 36.0g.

---

**👤 You:**
> "Calculate the percent yield for 2H2 + O2 -> 2H2O if I start with 4g of H2 and 32g of O2 and actually obtain 30g of H2O."

**🤖 AI Agent:**
> The percent yield is 83.33%.


## ❓ FAQ

**Q: How do I specify reactant amounts?**
Provide the reactant amounts as a JSON array of objects, where each object contains the formula and the mass in grams, such as `[{ "formula": "H2", "amount": 4 }]`.

**Q: What happens if my equation is unbalanced?**
The `validate_equation_and_masses` tool will detect if the equation is unbalanced and return an error reason.

**Q: Can I calculate the percent yield?**
Yes, you can use the `calculate_percent_yield` tool by providing the equation, reactant amounts, the actual yield mass, and the target product formula.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/stoichiometry-calculator](https://vinkius.com/ai-agent-connect/stoichiometry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stoichiometry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stoichiometry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stoichiometry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stoichiometry-calculator": {
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
