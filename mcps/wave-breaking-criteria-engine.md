# Wave Breaking Criteria Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-breaking-criteria-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-computing](../categories/scientific-computing.md)

Predict wave breaking height, type, and conditions using oceanographic models.

## Description
This MCP server provides specialized computational tools for oceanographic analysis. It uses McCowan and Miche models to determine when and how waves break based on water depth, wavelength, and beach slope. Use `check_breaking_conditions` for a full diagnostic, `get_breaking_height` to find depth-limited maximums, `analyze_breaker_type` to identify if a wave will be spilling, plunging, or surging, and `compare_criteria_models` to evaluate model variance.


## Available Tools (4)
- **analyze_breaker_type**: Identifies the physical character of the wave break (Spilling, Plunging, or Surging)
- **check_breaking_conditions**: A comprehensive diagnostic tool to determine if a specific wave is currently breaking or imminent
- **compare_criteria_models**: Compares the predictions of McCowan and Miche models to show the variance in breaking predictions
- **get_breaking_height**: Determines the maximum theoretical wave height possible at a specific location before breaking occurs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Breaking Criteria Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a wave with 5m height and 40m wavelength breaking in 10m of water with a 0.05 slope?"

**🤖 AI Agent:**
> No, the current wave height is below the predicted breaking threshold for these conditions.

---

**👤 You:**
> "What is the maximum wave height possible in 5 meters of water with a 0.03 beach slope?"

**🤖 AI Agent:**
> The maximum theoretical breaking height is 1.5 meters.

---

**👤 You:**
> "What type of breaker will a 3m wave with a 15m wavelength produce on a 0.1 slope?"

**🤖 AI Agent:**
> The wave will result in a plunging breaker.


## ❓ FAQ

**Q: What models are used for calculations?**
The engine utilizes McCowan's Criterion for depth-limited breaking and Miche's Criterion for steepness-based breaking.

**Q: How can I determine the type of wave break?**
You can use the `analyze_breaker_type` tool, which evaluates wave height, wavelength, and beach slope to classify the break as spilling, plunging, or surging.

**Q: Does this tool account for seafloor slope?**
Yes, the beach slope is a required input for most tools, including `get_breaking_height`, to ensure accurate predictions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-breaking-criteria-engine](https://vinkius.com/en/ai-agent-connect/wave-breaking-criteria-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Breaking Criteria Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-breaking-criteria-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Breaking Criteria Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-breaking-criteria-engine": {
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
