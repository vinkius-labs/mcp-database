# Reservoir Permeability Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-permeability-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Estimates permeability, skin factor, and wellbore storage from pressure transient data.

## Description
This MCP server provides specialized tools for Pressure Transient Analysis (PTA). It allows AI agents to interpret reservoir behavior by calculating critical parameters like permeability and skin factor. Use `analyze_drawdown` to evaluate active production phases, `analyze_buildup` to interpret pressure recovery after shut-in, and `calculate_storage_effect` to determine if wellbore storage is masking true reservoir response. The `get_skin_interpretation` tool provides qualitative insights into formation damage or stimulation.


## Available Tools (4)
- **calculate_storage_effect**: Determines if the wellbore storage is currently masking the true reservoir permeability
- **analyze_buildup**: Interprets pressure recovery data after a well has been shut in
- **analyze_drawdown**: Calculates reservoir characteristics during a period of active production/pressure reduction
- **get_skin_interpretation**: Provides a qualitative description of the reservoir condition based on the calculated skin factor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Permeability Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reservoir characteristics for a drawdown test with a flow rate of 500, pressure drop of 200, thickness of 50, viscosity of 1.2, radius of 0.1, and compressibility of 0.0001."

**🤖 AI Agent:**
> The estimated permeability is 150 mD, the skin factor is 2.5, and the wellbore storage coefficient is 0.00005.

---

**👤 You:**
> "What does a skin factor of -1.5 mean for my well?"

**🤖 AI Agent:**
> A skin factor of -1.5 indicates a stimulated well, meaning the flow has been enhanced near the wellbore.

---

**👤 You:**
> "Is the wellbore storage masking the reservoir response for a volume of 10, compressibility of 0.001, and radius of 0.1?"

**🤖 AI Agent:**
> The storage coefficient is 0.001, and it is not currently masking the true reservoir permeability.


## ❓ FAQ

**Q: What is the difference between drawdown and buildup analysis?**
Drawdown analysis measures pressure drop during active production, while buildup analysis measures pressure recovery after the well is shut in.

**Q: How can I interpret the skin factor?**
You can use the `get_skin_interpretation` tool to receive a qualitative description of the reservoir condition based on the calculated skin value.

**Q: Can this tool detect wellbore storage effects?**
Yes, the `calculate_storage_effect` tool determines if wellbore storage is currently masking the true reservoir permeability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-permeability-estimator](https://vinkius.com/en/ai-agent-connect/reservoir-permeability-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Permeability Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-permeability-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Permeability Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-permeability-estimator": {
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
