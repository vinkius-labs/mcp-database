# Concrete Sandblasting Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-sandblasting-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates abrasive mass, blasting duration, and equipment specifications for concrete surface preparation.

## Description
This MCP server provides precision calculation tools for concrete sandblasting projects. It determines the exact mass of abrasive material needed using `get_abrasive_requirements`, estimates operational time with `estimate_blasting_duration`, and recommends optimal equipment settings via `calculate_equipment_specs`. It also evaluates dust control needs through `check_containment_needs` to ensure safe and efficient surface preparation.


## Available Tools (4)
- **calculate_equipment_specs**: Recommends the necessary air pressure and nozzle configurations
- **check_containment_needs**: Evaluates the necessity and type of dust control and containment measures
- **estimate_blasting_duration**: Calculates the total time required to complete the surface preparation
- **get_abrasive_requirements**: Determines the total amount of abrasive material needed for the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Sandblasting Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much garnet do I need for 50m² of poor condition concrete with a heavy profile?"

**🤖 AI Agent:**
> For 50m² of poor condition concrete requiring a heavy profile, you will need 450kg of garnet, including 50kg of estimated waste.

---

**👤 You:**
> "What equipment do I need for a light profile using steel grit in a restricted environment?"

**🤖 AI Agent:**
> For a light profile with steel grit in a restricted environment, the recommended air pressure is 6.5 bar and the recommended nozzle size is 8mm.

---

**👤 You:**
> "How long will it take to blast 100m² of new concrete with a medium profile using a 10mm nozzle and garnet?"

**🤖 AI Agent:**
> Blasting 100m² of new concrete with a medium profile using a 10mm nozzle and garnet will take approximately 4.5 hours.


## ❓ FAQ

**Q: How do I calculate the amount of garnet I need?**
You can use the `get_abrasive_requirements` tool by providing the surface area, the concrete condition, the desired profile, and specifying garnet as the abrasive type.

**Q: Can this tool help with dust control planning?**
Yes, the `check_containment_needs` tool evaluates if containment is required based on the surface area and environmental constraints.

**Q: How is the blasting time estimated?**
The `estimate_blasting_duration` tool calculates time by analyzing the surface area, concrete condition, desired profile, abrasive type, and the specific nozzle size being used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-sandblasting-calculator](https://vinkius.com/ai-agent-connect/concrete-sandblasting-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Sandblasting Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-sandblasting-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Sandblasting Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-sandblasting-calculator": {
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
