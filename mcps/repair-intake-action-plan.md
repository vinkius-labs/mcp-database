# Repair Intake & Action Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-intake-action-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Converts property damage observations into prioritized repair briefs and safety protocols.

## Description
This MCP server acts as a triage engine for property damage. It maps symptoms to professional trades, evaluates safety hazards, and generates actionable repair briefs. Use `get_repair_triage` to create a prioritized plan, `validate_safety_status` to detect emergency stop conditions, `calculate_repair_priority` to rank jobs, and `get_trade_requirements` to prepare professionals for the task.


## Available Tools (4)
- **calculate_repair_priority**: Determines the numerical priority rank of the repair
- **get_repair_triage**: Converts raw user observations into a structured repair brief
- **get_trade_requirements**: Identifies what specific information or tools a professional in a specific trade will need
- **validate_safety_status**: Evaluates if the reported symptoms constitute a life-safety emergency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Intake & Action Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a leak in the kitchen under the sink and there is water near the outlet."

**🤖 AI Agent:**
> Emergency: A stop condition has been triggered due to water near electrical utilities. Please do not touch the outlet. Evacuate the area and shut off the main electricity if safe to do so. A plumber and electrician will be required.

---

**👤 You:**
> "There is a small crack in the living room ceiling."

**🤖 AI Agent:**
> The issue is classified as Structural. The priority is Medium. A structural specialist should inspect the ceiling to ensure no imminent failure is occurring.

---

**👤 You:**
> "The heater in the basement is making a loud banging noise."

**🤖 AI Agent:**
> The recommended trade is HVAC. The priority is High. A technician will need to inspect the heating unit and ventilation components.


## ❓ FAQ

**Q: How does the triage process work?**
The engine analyzes symptoms and utilities to determine the correct trade, such as Plumbing or Electrical, and checks for critical safety stop conditions.

**Q: What happens if a safety hazard is detected?**
If `validate_safety_status` triggers a stop condition, the system prioritizes immediate evacuation or utility shutdown over repair planning.

**Q: Can I use this to prepare a professional for a job?**
Yes, use `get_trade_requirements` to identify the specific tools, skills, and pre-repair checklists needed for the identified trade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-intake-action-plan](https://vinkius.com/en/ai-agent-connect/repair-intake-action-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Intake & Action Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-intake-action-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Intake & Action Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-intake-action-plan": {
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
