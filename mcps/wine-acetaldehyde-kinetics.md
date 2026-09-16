# Wine Acetaldehyde Kinetics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-acetaldehyde-kinetics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Models acetaldehyde formation and binding during fermentation to predict sensory risks.

## Description
This MCP server provides specialized tools for winemakers and enologists to model acetaldehyde behavior during fermentation. It allows AI agents to calculate sensory risks using `analyze_acetaldehyde_risk`, evaluate sulfur dioxide requirements with `calculate_so2_binding_capacity`, estimate yeast-driven production via `predict_metabolic_production`, and simulate the effects of oxygen exposure using `simulate_oxidation_impact`. By connecting to Vinkius Edge, your AI assistant can accurately predict free acetaldehyde levels, SO2 binding capacity, and the risk of sensory faults like bruised apple aromas.


## Available Tools (4)
- **calculate_so2_binding_capacity**: Evaluates how much additional SO2 is required to neutralize existing acetaldehyde
- **simulate_oxidation_impact**: Models how oxygen exposure will influence the transition of acetaldehyde into other compounds
- **analyze_acetaldehyde_risk**: Determines if the current wine conditions pose a sensory risk due to acetaldehyde levels
- **predict_metabolic_production**: Estimates the total amount of acetaldehyde the yeast will produce based on environmental factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Acetaldehyde Kinetics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the acetaldehyde risk for a fermentation using yeast strain 'Saccharomyces_cerevisiae' at 20°C with 30 mg/L SO2 and 5 units of oxygen exposure."

**🤖 AI Agent:**
> The current risk level is low. The free acetaldehyde concentration is 0.05 mg/L, which is well below the sensory threshold.

---

**👤 You:**
> "How much additional SO2 do I need if I have 10 mg/L of acetaldehyde and 25 mg/L of SO2 at a pH of 3.2?"

**🤖 AI Agent:**
> To neutralize the existing acetaldehyde, a required addition of 12.5 mg/L of SO2 is recommended.

---

**👤 You:**
> "Predict the acetaldehyde production for yeast strain 'Lalvin_EC100' at 18°C with 200 g/L of sugar."

**🤖 AI Agent:**
> The estimated total produced acetaldehyde is 15.4 mg/L with a production rate of 0.8 mg/L per hour.


## ❓ FAQ

**Q: How can I predict if my wine will have an acetaldehyde fault?**
You can use the `analyze_acetaldehyde_risk` tool. By providing the yeast strain, SO2 levels, oxygen exposure, and fermentation temperature, the tool determines if free acetaldehyde concentrations exceed sensory thresholds.

**Q: How does pH affect my SO2 requirements?**
The `calculate_so2_binding_capacity` tool accounts for pH. Lower pH levels change the proportion of molecular SO2, which directly impacts how effectively SO2 binds to acetaldehyde.

**Q: Can I model the impact of oxygen on my wine?**
Yes, the `simulate_oxidation_impact` tool models how oxygen exposure influences the transition of acetaldehyde into other compounds like acetic acid over a specific duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-acetaldehyde-kinetics](https://vinkius.com/en/ai-agent-connect/wine-acetaldehyde-kinetics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Acetaldehyde Kinetics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-acetaldehyde-kinetics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Acetaldehyde Kinetics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-acetaldehyde-kinetics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
