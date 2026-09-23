# Brine Water Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/brine-water-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise salt mass and water volume for specific salinity concentrations.

## Description
This MCP server provides precise mathematical tools for brine preparation. It allows AI agents to determine the exact mass of salt needed for a target salinity or the volume of water required to dissolve a specific amount of salt. Use `calculate_salt_mass` to find salt requirements for a given volume, or `calculate_water_for_salt` to find the necessary water volume. You can also use `verify_saturation_limit` to ensure your mixture remains physically possible and `get_salinity_from_masses` to check the resulting concentration of a known mixture.


## Available Tools (4)
- **calculate_salt_mass**: Determines exactly how much salt is needed to reach a target salinity for a specific volume of water
- **calculate_water_for_salt**: Determines how much water is required to dissolve a specific amount of salt at a specific target salinity
- **get_salinity_from_masses**: Calculates the resulting salinity percentage when a known amount of salt is added to a known amount of water
- **verify_saturation_limit**: Checks if a specific combination of salt and water is physically possible without the salt simply settling at the bottom


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brine Water Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much salt do I need to add to 50 liters of water to get a 3% salinity?"

**🤖 AI Agent:**
> To achieve a 3% salinity in 50 liters of water, you need to add 1.546 kg of salt.

---

**👤 You:**
> "I have 5kg of salt. How much water do I need for a 10% salinity solution?"

**🤖 AI Agent:**
> You need 45 liters of water to create a 10% salinity solution using 5kg of salt.

---

**👤 You:**
> "What is the salinity if I add 2kg of salt to 10 liters of water?"

**🤖 AI Agent:**
> The resulting salinity is 16.67%.


## ❓ FAQ

**Q: How do I calculate the salt needed for 10 liters of water at 5% salinity?**
You can use the `calculate_salt_mass` tool with a `waterVolume` of 10 and a `targetSalinity` of 5.

**Q: Can I check if my salt will dissolve in the water?**
Yes, use the `verify_saturation_limit` tool to check if the salt mass and water volume combination is physically possible.

**Q: What happens if I request a salinity that is too high?**
The tools will return an error if the requested salinity exceeds the physical saturation limits of water.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/brine-water-calculator](https://vinkius.com/en/ai-agent-connect/brine-water-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brine Water Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brine-water-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brine Water Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brine-water-calculator": {
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
