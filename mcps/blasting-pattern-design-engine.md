# Blasting Pattern Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blasting-pattern-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimized blast parameters for mining operations.

## Description
This MCP server provides specialized engineering tools for open-pit and underground mining design. It allows AI agents to calculate critical blast parameters including burden, spacing, and hole depth. Users can determine explosive loading requirements and timing sequences, while ensuring safety through vibration and flyrock risk assessments. Use `calculate_pattern_geometry` to define hole layouts and `validate_safety_constraints` to ensure compliance with site limits.


## Available Tools (4)
- **analyze_rock_suitability**: Evaluates if the selected explosive type is appropriate for the given rock properties
- **calculate_pattern_geometry**: Determines the spatial layout of the blast holes
- **compute_loading_and_timing**: Calculates the amount of explosive needed and the sequence of detonation
- **validate_safety_constraints**: Checks the design against vibration limits and flyrock risks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blasting Pattern Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the blast pattern geometry for a 10m bench height with a 3m burden and 4m spacing using a 102mm hole diameter."

**🤖 AI Agent:**
> The calculated pattern includes a burden of 3.0m, spacing of 4.0m, and a hole depth of 10.0m.

---

**👤 You:**
> "Is a charge weight of 50kg per delay safe for a structure 200m away with a vibration limit of 10mm/s and a 3m burden?"

**🤖 AI Agent:**
> Yes, the design is safe with a predicted vibration of 4.2mm/s and a Low flyrock risk.

---

**👤 You:**
> "Determine the explosive loading for a 12m hole with 102mm diameter, 0.85g/cm3 explosive density, and 3m stemming."

**🤖 AI Agent:**
> The total charge weight is 76.5kg with a timing sequence of [0, 25, 50, 75].


## ❓ FAQ

**Q: How do I calculate the hole layout?**
You can use the `calculate_pattern_geometry` tool by providing the burden, spacing, hole diameter, and bench height.

**Q: Can this tool check for safety risks?**
Yes, the `validate_safety_constraints` tool evaluates predicted vibration and flyrock risks based on your design parameters.

**Q: What explosive types are supported?**
The engine supports various types including ANFO, High-Density Emulsions, and Slurry Explosives through the `analyze_rock_suitability` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blasting-pattern-design-engine](https://vinkius.com/en/ai-agent-connect/blasting-pattern-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blasting Pattern Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blasting-pattern-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blasting Pattern Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blasting-pattern-design-engine": {
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
