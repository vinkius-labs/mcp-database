# Aquarium Marine Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aquarium-marine-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Deterministic dosing engine for marine aquarium water parameters.

## Description
This MCP server provides precise chemical dosing calculations for marine aquaria. It allows AI agents to determine exact amounts of products like calcium chloride or magnesium chloride needed to reach target levels. Use `calculate_dosing_requirements` to find specific dosing amounts, `calculate_salt_mix_needs` to prepare water changes, and `validate_parameter_stability` to ensure chemical shifts stay within safe biological limits.


## Available Tools (3)
- **calculate_dosing_requirements**: Determines the exact amount of various dosing products needed to reach target parameter levels
- **calculate_salt_mix_needs**: Determines the amount of salt required to adjust the salinity of a specific volume of water to a target level
- **validate_parameter_stability**: Checks if a planned dosing event or recent shift violates biological safety limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aquarium Marine Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 200L tank. Current calcium is 400ppm and I want it to be 440ppm. I have calcium chloride available. How much should I add?"

**🤖 AI Agent:**
> You need to add 12.5 grams of calcium chloride to reach your target of 440 ppm in a 200L tank.

---

**👤 You:**
> "How much salt do I need for a 50L water change to reach 35 ppt if my current salinity is 30 ppt?"

**🤖 AI Agent:**
> You need 250 grams of salt for a 50L volume to reach 35 ppt.

---

**👤 You:**
> "Is a calcium increase of 25 ppm in one day safe?"

**🤖 AI Agent:**
> No, a calcium increase of 25 ppm exceeds the safe daily limit of 20 ppm.


## ❓ FAQ

**Q: How do I know if my dosing is safe?**
You can use the `validate_parameter_stability` tool to check if your planned shifts in calcium, alkalinity, or magnesium exceed safe daily biological limits.

**Q: Can I calculate salt requirements for water changes?**
Yes, the `calculate_salt_mix_needs` tool calculates the exact grams of salt required to reach your target salinity for a specific volume.

**Q: What parameters can be calculated?**
The engine handles salinity, calcium, alkalinity, magnesium, nitrate, and phosphate levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aquarium-marine-calculator](https://vinkius.com/ai-agent-connect/aquarium-marine-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aquarium Marine Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aquarium-marine-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aquarium Marine Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aquarium-marine-calculator": {
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
