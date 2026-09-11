# Well Intervention Planning Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/well-intervention-planning-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Generates operational requirements, timelines, and contingency protocols for oil and gas well interventions.

## Description
This MCP server provides specialized planning capabilities for oil and gas well intervention operations. It allows AI agents to calculate precise equipment requirements using `get_equipment_requirements`, estimate operational timelines with `estimate_operational_timeline`, and generate safety protocols via `generate_contingency_protocols`. Additionally, it can verify if a chosen delivery method is safe for specific well conditions using `validate_method_suitability`. It supports planning for wireline, coiled tubing, and snubbing operations.


## Available Tools (4)
- **generate_contingency_protocols**: Provides a list of safety and recovery procedures based on potential risks
- **get_equipment_requirements**: Determines the specific hardware and tool strings needed for a planned intervention
- **validate_method_suitability**: Checks if a chosen intervention method is safe and capable of handling the specific well conditions
- **estimate_operational_timeline**: Calculates the expected duration for the entire intervention process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Intervention Planning Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What equipment do I need for a plug setting using wireline in a well with 3000 psi pressure and 150 degrees temperature?"

**🤖 AI Agent:**
> For a plug setting via wireline at 3000 psi and 150°F, you will require a specific tool string including a mechanical plug, a wireline unit with sufficient tension capacity, and pressure-rated lubricators rated above 3000 psi.

---

**👤 You:**
> "Estimate the time for a coiled tubing acid wash at 5000ft depth with 10 tools."

**🤖 AI Agent:**
> The total estimated duration for the coiled tubing acid wash at 5000ft is 42 hours, including mobilization, setup, active intervention, and teardown.

---

**👤 You:**
> "What should I do if a pressure spike occurs during a snubbing operation?"

**🤖 AI Agent:**
> In the event of a pressure spike during snubbing, the primary protocol is to immediately halt injection and stabilize the wellbore pressure using the snubbing unit's control system.


## ❓ FAQ

**Q: What intervention methods are supported?**
The engine supports wireline, coiled tubing, and snubbing operations.

**Q: How can I check if a method is safe for my well?**
You can use the `validate_method_suitability` tool to check if a method is capable of handling specific pressure and temperature conditions.

**Q: Can this tool help with equipment selection?**
Yes, the `get_equipment_requirements` tool determines the specific hardware, tool strings, and pressure ratings needed for your planned task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/well-intervention-planning-engine](https://vinkius.com/en/ai-agent-connect/well-intervention-planning-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Intervention Planning Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-intervention-planning-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Intervention Planning Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-intervention-planning-engine": {
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
