# Concrete Heat of Hydration Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-heat-of-hydration-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates thermal stress, peak temperature, and cooling needs for mass concrete.

## Description
This MCP server provides specialized tools for managing thermal risks in mass concrete construction. It uses an adiabatic temperature rise model to predict how cement hydration affects core temperatures. Engineers can use `calculate_peak_temperature` to find maximum heat levels, `evaluate_thermal_risk` to assess cracking potential based on temperature gradients, and `determine_cooling_requirements` to decide if internal cooling pipes are necessary. The server also includes `simulate_mix_design` to compare how fly ash replacement impacts the heat profile.


## Available Tools (4)
- **calculate_peak_temperature**: Determines the maximum theoretical temperature the concrete core will reach
- **determine_cooling_requirements**: Identifies if internal cooling is necessary and what type of cooling is needed
- **evaluate_thermal_risk**: Assesses the risk of cracking by comparing temperature differences and stresses
- **simulate_mix_design**: Allows the user to compare how different cement/fly ash combinations affect the heat profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Heat of Hydration Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will be the peak temperature for 350kg/m³ of Type I cement?"

**🤖 AI Agent:**
> The calculated peak temperature for 350kg/m³ of Type I cement is 62.5°C, with a total adiabatic rise of 58.2°C.

---

**👤 You:**
> "Is there a cracking risk for a 5m³ element with a 60°C core temperature and 20°C ambient temperature?"

**🤖 AI Agent:**
> The risk level is High. The temperature gradient is 40°C and the calculated thermal stress is 12.4 MPa, which exceeds standard safety thresholds.

---

**👤 You:**
> "Should I use cooling pipes if my max allowable stress is 10 MPa?"

**🤖 AI Agent:**
> Yes, cooling is required. The calculated thermal stress exceeds your 10 MPa limit, and the recommended method is Internal Cooling Pipes.


## ❓ FAQ

**Q: How does this tool help prevent concrete cracking?**
By using `evaluate_thermal_risk`, you can identify if the temperature gradient between the core and the surface exceeds safe limits, allowing you to implement mitigation strategies like insulation or cooling before cracking occurs.

**Q: Can I simulate the effect of fly ash?**
Yes, the `simulate_mix_design` tool allows you to compare different cement and fly ash combinations to see how they affect the total heat release and peak temperature.

**Q: What determines if I need cooling pipes?**
The `determine_cooling_requirements` tool evaluates the calculated thermal stress and temperature gradient against your specific project limits to recommend if internal cooling pipes are required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-heat-of-hydration-analyzer](https://vinkius.com/ai-agent-connect/concrete-heat-of-hydration-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Heat of Hydration Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-heat-of-hydration-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Heat of Hydration Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-heat-of-hydration-analyzer": {
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
