# Terephthalic Acid Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/terephthalic-acid-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing Purified Terephthalic Acid (PTA) production plants.

## Description
This MCP server provides specialized engineering calculations for designing a Purified Terephthalic Acid (PTA) plant. It allows AI agents to model the entire production chain from p-xylene oxidation to final purification. Users can use `calculate_oxidation_reactor` to determine reactor sizing, `design_catalyst_system` to optimize chemical compositions, `evaluate_purification_stage` to manage 4-CBA impurity levels, and `estimate_solvent_recovery` to ensure acetic acid efficiency. It is designed to bridge chemical engineering expertise with AI-driven process optimization.


## Available Tools (4)
- **evaluate_purification_stage**: Calculates the purification requirements to meet specific product grades
- **calculate_oxidation_reactor**: Determines the necessary reactor size and operating conditions based on feed availability
- **design_catalyst_system**: Specifies the required catalyst composition and concentration for the oxidation
- **estimate_solvent_recovery**: Calculates the efficiency and mass of acetic acid that must be recovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terephthalic Acid Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor requirements for 50,000 tons of PTA capacity with 100,000 tons of p-xylene available at 180 degrees."

**🤖 AI Agent:**
> The required reactor volume is 450 cubic meters with a temperature setpoint of 180°C, yielding an estimated 48,500 tons of PTA.

---

**👤 You:**
> "What catalyst composition is needed for a 450 cubic meter reactor to achieve 99.9% purity?"

**🤖 AI Agent:**
> To achieve 99.9% purity in a 450 cubic meter reactor, the system requires a cobalt concentration of 0.05 and a manganese concentration of 0.03.

---

**👤 You:**
> "Estimate the solvent recovery for 5000 tons of acetic acid with a 2% impurity loss rate."

**🤖 AI Agent:**
> The system will recover 4,900 tons of acetic acid, requiring 100 tons of makeup solvent.


## ❓ FAQ

**Q: How do I calculate the reactor size?**
You can use the `calculate_oxidation_reactor` tool by providing the available p-xylene mass, the target annual capacity, and the desired reaction temperature.

**Q: Can this tool help manage 4-CBA impurities?**
Yes, the `evaluate_purification_stage` tool specifically calculates the hydrogen consumption and filtration cycles needed to reach your target 4-CBA concentration.

**Q: How is the catalyst system determined?**
The `design_catalyst_system` tool determines the required cobalt and manganese concentrations based on your reactor volume and the target purity of the PTA.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/terephthalic-acid-plant-designer](https://vinkius.com/en/ai-agent-connect/terephthalic-acid-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terephthalic Acid Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `terephthalic-acid-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terephthalic Acid Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terephthalic-acid-plant-designer": {
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
