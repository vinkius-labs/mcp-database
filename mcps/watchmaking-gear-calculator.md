# Watchmaking Gear Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/watchmaking-gear-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Deterministic engine for horological gear train ratios, beat rates, and power reserves.

## Description
This MCP server provides precise mechanical calculations for horological movements. It allows AI agents to determine exact gear ratios per stage, total train ratios, and beat rates (vibrations per hour) for Swiss lever escapements. Users can also estimate power reserves based on barrel turns and validate escapement stability using balance wheel inertia. Use `calculate_gear_train` to find the timing of a movement, `estimate_power_reserve` to calculate operational duration, and `validate_escapement_physics` to ensure the configuration is theoretically sound.


## Available Tools (3)
- **calculate_gear_train**: 
- **estimate_power_reserve**: 
- **validate_escapement_physics**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Watchmaking Gear Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the beat rate for a movement with a 60-tooth barrel, 60-tooth center wheel, 6-tooth center pinion, 60-tooth third wheel, 6-tooth third pinion, 60-tooth fourth wheel, 6-tooth fourth pinion, 15-tooth escape wheel, and 6-tooth escape pinion."

**🤖 AI Agent:**
> The total train ratio is 100, and the beat rate is 3,000 vph.

---

**👤 You:**
> "Estimate the power reserve for a movement with a total train ratio of 400 and 30 barrel turns."

**🤖 AI Agent:**
> The estimated power reserve is 7.5 hours.

---

**👤 You:**
> "Is an escapement with 15 escape wheel teeth and a balance wheel inertia of 0.05 stable?"

**🤖 AI Agent:**
> Yes, the escapement configuration is stable with a theoretical frequency of 4Hz.


## ❓ FAQ

**Q: How is the beat rate calculated?**
The beat rate is the product of the total train ratio and the number of escape wheel teeth, multiplied by two for the Swiss lever escapement mechanics.

**Q: What happens if a pinion is larger than its driving wheel?**
The `calculate_gear_train` tool will flag this as a mathematically and mechanically impossible gear mesh.

**Q: Can I estimate how long a watch will run?**
Yes, by using the `estimate_power_reserve` tool with the total train ratio and the number of barrel turns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/watchmaking-gear-calculator](https://vinkius.com/ai-agent-connect/watchmaking-gear-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Watchmaking Gear Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `watchmaking-gear-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Watchmaking Gear Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "watchmaking-gear-calculator": {
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
