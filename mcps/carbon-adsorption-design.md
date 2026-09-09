# Carbon Adsorption Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/carbon-adsorption-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design carbon adsorption circuits for gold recovery processes.

## Description
This MCP server provides engineering tools to design carbon adsorption circuits used in gold recovery. It allows for precise calculation of critical operational parameters including carbon inventory, tank sizing, and replenishment rates. Use `calculate_carbon_inventory` to determine required carbon mass, `design_tank_dimensions` for vessel sizing, `calculate_advance_rate` for replenishment speed, and `predict_isotherm_loading` to model gold uptake based on adsorption isotherms.


## Available Tools (4)
- **calculate_advance_rate**: Calculates how fast carbon must be replenished or moved to maintain efficiency
- **calculate_carbon_inventory**: Determines the total mass of activated carbon required for the circuit
- **design_tank_dimensions**: Calculates the physical volume required for the adsorption vessels
- **predict_isotherm_loading**: Predicts how much gold will be on the carbon at equilibrium for a given concentration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbon Adsorption Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much carbon do I need for a throughput of 100 m3/h with 5 mg/L gold and a capacity of 10 mg/g?"

**🤖 AI Agent:**
> The required carbon inventory is 50 kg with a safety factor of 1.2, totaling 60 kg of carbon.

---

**👤 You:**
> "What size tank is needed for 50 m3/h throughput with a 2-hour contact time and 40% carbon holdup?"

**🤖 AI Agent:**
> The required total tank volume is 250 m3, consisting of 150 m3 of solution and 100 m3 of carbon.

---

**👤 You:**
> "Predict the gold loading for a feed concentration of 2 mg/L with an isotherm constant of 0.5."

**🤖 AI Agent:**
> The predicted equilibrium gold loading is 1.0 mg/g.


## ❓ FAQ

**Q: How do I calculate the required carbon mass?**
You can use the `calculate_carbon_inventory` tool by providing the gold concentration, the loading capacity, and the solution throughput.

**Q: Can I size my adsorption tanks with this tool?**
Yes, the `design_tank_dimensions` tool calculates the required volume based on throughput, contact time, and carbon holdup.

**Q: What is the purpose of the advance rate calculation?**
The `calculate_advance_rate` tool determines how quickly carbon must be moved or replaced to maintain efficient gold capture.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/carbon-adsorption-design](https://vinkius.com/ai-agent-connect/carbon-adsorption-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbon Adsorption Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbon-adsorption-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbon Adsorption Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbon-adsorption-design": {
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
