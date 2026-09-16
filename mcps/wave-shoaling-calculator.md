# Wave Shoaling Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-shoaling-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculates wave height changes and shoaling coefficients as waves approach shallow water.

## Description
This MCP server provides specialized tools for oceanographic analysis of wave shoaling. It allows AI agents to calculate how wave height increases as waves move from deep water into shallower regions due to energy conservation. Using `calculate_shoaling_parameters`, agents can determine the shoaling coefficient and wavelength reduction. The server also includes `analyze_wave_regime` to identify if waves are in deep, intermediate, or shallow water, and `predict_breaking_height` to estimate when a wave will become unstable and break.


## Available Tools (4)
- **analyze_wave_regime**: Identifies if a wave is behaving in deep, intermediate, or shallow water based on depth and wavelength
- **calculate_shoaling_parameters**: Determines the primary coefficients and physical changes occurring during the shoaling process
- **get_energy_flux_ratio**: Compares the energy transmission capability between deep and shallow water
- **predict_breaking_height**: Estimates the maximum height a wave can reach before it becomes unstable and breaks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Shoaling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shoaling parameters for a wave with a height of 2m, a period of 10s, in 5m of water."

**🤖 AI Agent:**
> The shoaling coefficient is 1.15, the new wave height is 2.3m, and the wavelength reduction is 4.2m.

---

**👤 You:**
> "Is a wave with a 10s period in 20m of water in deep or shallow water?"

**🤖 AI Agent:**
> The wave is in the intermediate water regime.

---

**👤 You:**
> "What is the maximum stable height for a wave in 3m of water if the deep water height was 1.5m?"

**🤖 AI Agent:**
> The maximum stable height is 2.1m, leaving a safety margin of 0.6m.


## ❓ FAQ

**Q: What is wave shoaling?**
Wave shoaling is the process where wave height increases as waves move into shallower water, driven by the conservation of energy flux as wave speed changes.

**Q: How can I determine if a wave is about to break?**
You can use the `predict_breaking_height` tool to estimate the maximum stable height a wave can reach before it becomes unstable and breaks.

**Q: What wave regimes are supported?**
The `analyze_wave_regime` tool identifies whether a wave is in a deep, intermediate, or shallow water regime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-shoaling-calculator](https://vinkius.com/en/ai-agent-connect/wave-shoaling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Shoaling Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-shoaling-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Shoaling Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-shoaling-calculator": {
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
