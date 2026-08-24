# Distillation Proof Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/distillation-proof-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Deterministic tools for alcohol proof correction, distillation stage identification, and volume-based cuts.

## Description
This MCP server provides a deterministic toolset for distillers to manage alcohol concentration accuracy. Use `get_corrected_proof` to adjust hydrometer readings for temperature deviations using TTB-standardized logic. Identify your current distillation phase with `identify_distillation_stage`, or calculate precise volumes for heads, hearts, and tails using `calculate_cuts_volume`. You can also determine exact water requirements for bottling with `calculate_dilution_needs`.


## Available Tools (4)
- **calculate_cuts_volume**: Calculates the specific volumes of heads, hearts, and tails produced from a total distillate volume
- **calculate_dilution_needs**: Determines how much water is required to dilute a high-proof spirit to a desired bottling strength
- **get_corrected_proof**: Calculates the accurate alcohol concentration and US proof by adjusting an observed hydrometer reading for temperature
- **identify_distillation_stage**: Determines which phase of distillation a liquid is likely in based on its concentration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Distillation Proof Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My hydrometer reads 40% ABV at 75°F. What is the corrected US proof at 60°F?"

**🤖 AI Agent:**
> The corrected ABV is 40.8% and the US proof is 81.6.

---

**👤 You:**
> "I have 5 liters of distillate at 65% ABV. How much volume will be in my hearts cut?"

**🤖 AI Agent:**
> The hearts cut will be 3.25 liters.

---

**👤 You:**
> "I have 2 liters of 80% ABV spirit. How much water do I need to add to reach 40% ABV?"

**🤖 AI Agent:**
> You need to add 2 liters of water to reach a final total volume of 4 liters.


## ❓ FAQ

**Q: How does temperature affect my hydrometer reading?**
Hydrometer readings change based on liquid density, which is affected by temperature. The `get_corrected_proof` tool adjusts your observed ABV to a standard calibration temperature to ensure accuracy.

**Q: Can I calculate my cuts using this tool?**
Yes, by providing the total volume and ABV, `calculate_cuts_volume` provides the specific volumes for heads, hearts, and tails.

**Q: How do I know if I am in a stripping run or a spirit run?**
The `identify_distillation_stage` tool analyzes your ABV to determine if you are in a stripping run (typically ~30% ABV) or a spirit run (typically 60-80% ABV).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/distillation-proof-calculator](https://vinkius.com/ai-agent-connect/distillation-proof-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Distillation Proof Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `distillation-proof-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Distillation Proof Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "distillation-proof-calculator": {
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
