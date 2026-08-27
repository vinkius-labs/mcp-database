# Wine SO2 Equilibrium Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-so2-equilibrium-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate SO2 speciation and microbial stability in wine.

## Description
This MCP server provides winemakers with precise tools to manage sulfur dioxide (SO2) levels. By analyzing pH, alcohol, and temperature, it calculates the distribution of SO2 species, specifically identifying the molecular SO2 available for antimicrobial protection. Use `get_current_speciation` to see the current breakdown of free and bound SO2, `calculate_required_addition` to determine how much more SO2 is needed to reach a target molecular level, and `evaluate_stability_risk` to assess microbial spoilage risks.


## Available Tools (4)
- **calculate_required_addition**: Determine how much additional total SO2 must be added to reach a specific target of molecular SO2
- **evaluate_stability_risk**: Assess whether the current SO2 levels are sufficient to prevent microbial spoilage
- **get_current_speciation**: Determine the current distribution of SO2 species based on existing wine parameters
- **get_equilibrium_constants**: Retrieve the environmental constants used for the specific temperature and alcohol conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine SO2 Equilibrium Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current SO2 speciation for a wine with pH 3.5, 13% alcohol, 20°C, and 40 mg/L total SO2?"

**🤖 AI Agent:**
> The current speciation is: Free SO2: 25.4 mg/L, Molecular SO2: 4.2 mg/L, Bound SO2: 14.6 mg/L, Total SO2: 40.0 mg/L.

---

**👤 You:**
> "How much SO2 should I add to reach 0.8 mg/L molecular SO2 if my current pH is 3.6, alcohol is 12%, temperature is 18°C, and total SO2 is 30 mg/L?"

**🤖 AI Agent:**
> To reach a target of 0.8 mg/L molecular SO2, you need to add 12.5 mg/L of total SO2.

---

**👤 You:**
> "Is my wine stable with pH 3.8, 14% alcohol, 22°C, and 35 mg/L total SO2?"

**🤖 AI Agent:**
> The current molecular SO2 is 0.5 mg/L, which is below the 0.8 mg/L threshold. The risk level is Moderate.


## ❓ FAQ

**Q: What is the purpose of the `get_current_speciation` tool?**
It determines the current distribution of SO2 species, including free, molecular, and bound SO2, based on the wine's pH, alcohol, and temperature.

**Q: How do I know if my wine is at risk of spoilage?**
You can use the `evaluate_stability_risk` tool to assess if your current molecular SO2 levels are sufficient to prevent microbial spoilage.

**Q: Can I calculate how much SO2 to add?**
Yes, the `calculate_required_addition` tool calculates the exact amount of total SO2 needed to reach your desired target of molecular SO2.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-so2-equilibrium-calculator](https://vinkius.com/ai-agent-connect/wine-so2-equilibrium-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine SO2 Equilibrium Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-so2-equilibrium-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine SO2 Equilibrium Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-so2-equilibrium-calculator": {
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
