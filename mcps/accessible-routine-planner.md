# Accessible Routine Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-routine-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates phased routine transition plans that respect accessibility needs and support networks.

## Description
This MCP server provides a structured engine for managing life transitions. It reconciles upcoming changes with existing accessibility requirements, support networks, and logistical constraints. Users can use `generate_routine_transition` to create a phased plan, `validate_support_capacity` to ensure their network can handle the load, `check_location_accessibility` to verify physical environments, and `calculate_transition_pacing` to determine the optimal speed of change based on personal priorities.


## Available Tools (4)
- **calculate_transition_pacing**: Determines optimal duration between phases based on priorities
- **validate_support_capacity**: Checks if the support network is sufficient for the required tasks
- **check_location_accessibility**: Verifies if locations can support specific access dependencies
- **generate_routine_transition**: Generates a phased routine transition plan based on life changes and constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Routine Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am moving to a new house next month and need a plan that minimizes physical fatigue."

**🤖 AI Agent:**
> I have generated a phased transition plan. The first phase focuses on preparation and gathering equipment, with a slower pace to ensure your fatigue levels remain low as requested.

---

**👤 You:**
> "Will my current support network be able to help me with my new job transition?"

**🤖 AI Agent:**
> Based on the tasks identified, your current support network is sufficient to cover the primary transition requirements.

---

**👤 You:**
> "Is the new office accessible for someone using a wheelchair?"

**🤖 AI Agent:**
> The location is accessible, as the provided equipment meets your specific access dependencies.


## ❓ FAQ

**Q: How does the tool handle accessibility needs?**
The `check_location_accessibility` tool specifically verifies if your chosen locations can support your specific access dependencies using your available equipment.

**Q: Can I adjust how fast my routine changes?**
Yes, you can use `calculate_transition_pacing` to determine the optimal duration between phases based on your specific priorities, such as minimizing fatigue.

**Q: How do I know if my support network is enough?**
You can use `validate_support_capacity` to check if your available people and services are sufficient to handle the tasks identified in your transition plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-routine-planner](https://vinkius.com/en/ai-agent-connect/accessible-routine-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Routine Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-routine-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Routine Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-routine-planner": {
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
