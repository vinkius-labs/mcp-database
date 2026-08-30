# Solution Concentration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/solution-concentration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate molarity, molality, mass percent, and other chemical concentrations.

## Description
This MCP server provides a specialized engine for chemical concentration calculations. It allows AI agents to determine precise values for molarity (M), molality (m), normality (N), mass percent, ppm, ppb, and mole fraction. By using tools like `calculate_molarity` and `calculate_mass_based_concentrations`, agents can bridge the gap between raw solute/solvent data and actionable chemical analysis. The engine handles complex conversions, including density-adjusted molarity calculations.


## Available Tools (5)
- **calculate_mass_based_concentrations**: Calculate mass-based ratios including percent, ppm, and ppb
- **calculate_density_adjusted_molarity**: Convert volume-based solvent measurements to molarity using solution density
- **calculate_molality**: Determine the molal concentration of a solution
- **calculate_molarity**: Determine the molar concentration of a solution
- **calculate_mole_fraction**: Determine the ratio of solute moles to total moles in a solution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solution Concentration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the molarity of a solution with 5.85g of NaCl in 0.5L of solution, given NaCl has a molecular weight of 58.44 g/mol?"

**🤖 AI Agent:**
> The molarity of the solution is 0.2 M.

---

**👤 You:**
> "Calculate the mass percent of 10g of solute in 90g of solvent."

**🤖 AI Agent:**
> The mass percent is 10%.

---

**👤 You:**
> "Find the mole fraction of 2 moles of solute in a solution where the solvent has 8 moles."

**🤖 AI Agent:**
> The mole fraction is 0.2 and the mole percent is 20%.


## ❓ FAQ

**Q: What units can this tool calculate?**
The tool calculates molarity, molality, normality, mass percent, ppm, ppb, and mole fraction.

**Q: How do I calculate molarity?**
You can use the `calculate_molarity` tool by providing the solute mass, solution volume, and molecular weight.

**Q: Does it support mass-based ratios?**
Yes, the `calculate_mass_based_concentrations` tool provides mass percent, ppm, and ppb.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/solution-concentration-calculator](https://vinkius.com/ai-agent-connect/solution-concentration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solution Concentration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solution-concentration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solution Concentration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solution-concentration-calculator": {
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
