# Natural Gas Dehydration Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/natural-gas-dehydration-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing glycol absorption and molecular sieve adsorption dehydration systems.

## Description
This MCP provides specialized engineering tools for natural gas dehydration design. It allows for the calculation of TEG-based glycol absorption systems using `design_glycol_system` to determine circulation rates, contactor diameters, and reboiler duties. For solid-phase adsorption, `design_molecular_sieve_system` calculates required desiccant bed dimensions. Additionally, users can determine theoretical limits with `calculate_equilibrium_water_content` and estimate environmental impact using `estimate_btex_loss`.


## Available Tools (4)
- **design_molecular_sieve_system**: Calculates the required desiccant bed dimensions for adsorption-based dehydration
- **estimate_btex_loss**: Estimates the amount of aromatic hydrocarbons lost during the glycol regeneration process
- **design_glycol_system**: Calculates the physical and operational requirements for a TEG-based dehydration unit
- **calculate_equilibrium_water_content**: Determines the theoretical maximum water content in the gas at specific conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Natural Gas Dehydration Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a glycol dehydration system for 500,000 scfh of gas with 60 lb/MMscf water content, targeting a 30F dew point at 800 psia and 100F, using 95% pure glycol."

**🤖 AI Agent:**
> The required glycol circulation rate is 12.5 gallons per hour, the contactor diameter is 36 inches, and the reboiler duty is 45,000 BTUs per hour.

---

**👤 You:**
> "Calculate the molecular sieve bed size for 1,000,000 scfh of gas, 100 lb/MMscf water, 30F target dew point, 1000 psia, 110F, and a 12-hour cycle time."

**🤖 AI Agent:**
> The required desiccant bed has a volume of 45 cubic feet, a diameter of 48 inches, a height of 72 inches, and requires 1,200 pounds of desiccant.

---

**👤 You:**
> "What is the equilibrium water content at 500 psia and 80F?"

**🤖 AI Agent:**
> The theoretical maximum water content at 500 psia and 80F is 42.5 lb/MMscf.


## ❓ FAQ

**Q: What is the difference between the two design methods?**
The tool supports glycol absorption, which uses a liquid desiccant, and molecular sieve adsorption, which uses solid desiccant beads.

**Q: How do I calculate the contactor size for a glycol system?**
You can use the `design_glycol_system` tool, which provides the required contactor diameter based on your gas flow rate and operating conditions.

**Q: Can I estimate environmental emissions?**
Yes, the `estimate_btex_loss` tool allows you to estimate the amount of aromatic hydrocarbons lost during the glycol regeneration process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/natural-gas-dehydration-designer](https://vinkius.com/en/ai-agent-connect/natural-gas-dehydration-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Natural Gas Dehydration Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `natural-gas-dehydration-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Natural Gas Dehydration Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "natural-gas-dehydration-designer": {
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
