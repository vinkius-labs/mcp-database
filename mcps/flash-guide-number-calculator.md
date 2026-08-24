# Flash Guide Number Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/flash-guide-number-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calculators](../categories/calculators.md)

Calculate photographic exposure, power adjustments, and flash stacking requirements.

## Description
This MCP server provides deterministic tools for photographic exposure calculations based on flash Guide Numbers (GN). It allows AI agents to calculate the required aperture using `get_exposure_requirements`, determine effective Guide Numbers at specific power levels with `get_power_adjusted_gn`, and calculate the combined light output of multiple units using `get_stacked_flash_gn`. It is designed to handle ISO sensitivity adjustments and the Inverse Square Law for precise flash photography planning.


## Available Tools (3)
- **get_exposure_requirements**: 
- **get_power_adjusted_gn**: 
- **get_stacked_flash_gn**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flash Guide Number Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a flash with a GN of 120 at ISO 100. I am 5 meters away from my subject at ISO 400. What f-stop should I use?"

**🤖 AI Agent:**
> The required aperture is f/6.

---

**👤 You:**
> "My flash has a GN of 100. What is the effective GN if I use it at 1/4 power?"

**🤖 AI Agent:**
> The effective Guide Number at 1/4 power is 50.

---

**👤 You:**
> "If I use 4 flash units, each with a GN of 60, what is the total effective GN?"

**🤖 AI Agent:**
> The total effective Guide Number for 4 units is 120.


## ❓ FAQ

**Q: How do I calculate the correct aperture for my flash?**
You can use the `get_exposure_requirements` tool. Provide the Guide Number at ISO 100, the distance to your subject, and your target ISO to receive the required f-stop.

**Q: Can I calculate the effect of using half power?**
Yes, use the `get_power_adjusted_gn` tool by providing the Guide Number at ISO 100 and setting the power fraction to 0.5.

**Q: What happens when I use multiple flashes at once?**
When multiple flashes fire simultaneously, their light combines. Use `get_stacked_flash_gn` to find the total effective Guide Number based on the number of units used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/flash-guide-number-calculator](https://vinkius.com/ai-agent-connect/flash-guide-number-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flash Guide Number Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flash-guide-number-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flash Guide Number Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flash-guide-number-calculator": {
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
