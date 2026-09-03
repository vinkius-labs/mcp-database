# Scaffolding Load Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/scaffolding-load-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates safe working loads, bracing requirements, and stability for scaffolding.

## Description
This MCP server provides structural engineering calculations for scaffolding configurations. It allows AI agents to determine the maximum safe load per square meter using `get_safe_working_load`, identify necessary diagonal patterns with `calculate_bracing_requirements`, find maximum tie spacing via `determine_tie_spacing`, and evaluate overturning risks with `check_stability_limits`.


## Available Tools (4)
- **calculate_bracing_requirements**: Identifies the necessary diagonal bracing pattern required to maintain lateral stability
- **check_stability_limits**: Evaluates if the current configuration is at risk of overturning or structural failure
- **determine_tie_spacing**: Calculates the maximum allowable distance between wall ties to ensure the scaffold does not tip
- **get_safe_working_load**: Determines the maximum allowable pressure per square meter the scaffold can safely carry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scaffolding Load Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the safe working load for a Supported scaffold that is 5m high, has a 2m bay length, and 10kN leg capacity?"

**🤖 AI Agent:**
> The maximum safe load for this configuration is 2.5 kN/m².

---

**👤 You:**
> "Calculate the tie spacing for a 10m high Supported scaffold with a wind load of 0.5 kN/m²."

**🤖 AI Agent:**
> The maximum horizontal tie spacing is 4.0m and the vertical spacing is 4.5m.

---

**👤 You:**
> "Is a Mobile scaffold with 4m height and 5kN leg capacity stable under 0.8 kN/m² wind load?"

**🤖 AI Agent:**
> The configuration is stable with a safety factor of 1.8.


## ❓ FAQ

**Q: How do I calculate the safe working load?**
You can use the `get_safe_working_load` tool by providing the scaffold type, height, bay length, and leg load capacity.

**Q: Can this tool check if my scaffold is stable?**
Yes, the `check_stability_limits` tool evaluates the safety factor and potential failure modes like overturning.

**Q: What scaffold types are supported?**
The server supports Supported, Suspended, and Mobile scaffold types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/scaffolding-load-capacity-calculator](https://vinkius.com/ai-agent-connect/scaffolding-load-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scaffolding Load Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scaffolding-load-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scaffolding Load Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scaffolding-load-capacity-calculator": {
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
