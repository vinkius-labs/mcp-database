# CO2 Flood Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/co2-flood-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design CO2 Enhanced Oil Recovery (EOR) projects by calculating MMP, injection strategies, and recovery estimates.

## Description
This MCP server provides specialized engineering tools for Carbon Dioxide (CO2) Enhanced Oil Recovery (EOR) design. It allows AI agents to model reservoir conditions and optimize injection parameters. Use `calculate_mmp` to find the Minimum Miscibility Pressure, `design_injection_strategy` to determine optimal WAG ratios and injection rates, `estimate_recovery_and_recycle` to predict oil yield and CO2 recycling needs, and `assess_corrosion_risk` to evaluate equipment integrity based on temperature and CO2 source.


## Available Tools (4)
- **assess_corrosion_risk**: Evaluates the integrity risks posed by CO2 and water interaction
- **calculate_mmp**: Determines the Minimum Miscibility Pressure required for the specific oil-CO2 mixture
- **design_injection_strategy**: Determines the optimal injection rates and the Water-Alternating-Gas (WAG) ratio
- **estimate_recovery_and_recycle**: Predicts the total oil recovered and the amount of CO2 that will need to be recycled


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CO2 Flood Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum miscibility pressure for an oil with light hydrocarbon makeup at 5000 feet and 180 degrees Fahrenheit?"

**🤖 AI Agent:**
> The calculated Minimum Miscibility Pressure is 2450 psi, and the current conditions are likely to support miscibility.

---

**👤 You:**
> "Estimate the oil recovery for a reservoir with a volume of 10,000,000 barrels, an injection rate of 5000 barrels per day, and a WAG ratio of 1.5."

**🤖 AI Agent:**
> The estimated total recovery is 1,250,000 barrels of oil, with a daily CO2 recycle requirement of 450 barrels.

---

**👤 You:**
> "What is the corrosion risk for a reservoir at 220 degrees Fahrenheit using industrial capture CO2 at an injection rate of 2000 barrels per day?"

**🤖 AI Agent:**
> The corrosion risk level is High. It is recommended to use corrosion-resistant alloys (CRA) and continuous chemical inhibitor injection.


## ❓ FAQ

**Q: How do I calculate the Minimum Miscibility Pressure?**
You can use the `calculate_mmp` tool by providing the oil composition, reservoir depth, and reservoir temperature.

**Q: Can this tool help with corrosion management?**
Yes, the `assess_corrosion_risk` tool evaluates integrity risks and provides mitigation strategies based on reservoir temperature and CO2 source.

**Q: What information is needed for injection strategy design?**
To use `design_injection_strategy`, you need the calculated MMP, the reservoir depth, and the specific oil composition.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/co2-flood-design-tool](https://vinkius.com/en/ai-agent-connect/co2-flood-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CO2 Flood Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `co2-flood-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CO2 Flood Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "co2-flood-design-tool": {
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
