# GYROTONIC® Expansion Series Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gyrotonic-expansion-series-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates structured GYROTONIC® expansion series protocols based on client level and equipment.

## Description
This MCP server provides a specialized planning engine for GYROTONIC® expansion series. It allows AI agents to generate complete session protocols, including exercise sequences, repetition ranges, and breathing patterns. Users can use `get_session_plan` to create a full routine, `get_exercise_details` for technical movement specifics, `validate_progression_path` to ensure physiological safety, and `get_equipment_capabilities` to understand what movements are possible on specific apparatus like the Pulley Tower or Handle Unit.


## Available Tools (4)
- **get_equipment_capabilities**: Retrieves the available exercises and movement focus for a specific piece of equipment
- **get_exercise_details**: Provides specific technical details for an individual exercise within a series
- **get_session_plan**: Generates a complete, structured session protocol for a single client
- **validate_progression_path**: Checks if a sequence of exercises follows a valid physiological progression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GYROTONIC® Expansion Series Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 45-minute mobility session for an intermediate client using the Pulley Tower."

**🤖 AI Agent:**
> The session will consist of a 45-minute expansion series focused on spinal mobility, featuring specific curvilinear movements on the Pulley Tower with guided breathing patterns.

---

**👤 You:**
> "What are the technical details for the 'Spinal Articulation' exercise for a beginner?"

**🤖 AI Agent:**
> For a beginner, 'Spinal Articulation' involves 8 to 10 repetitions focusing on slow, controlled circular movements with deep inhalation during expansion and exhalation during contraction.

---

**👤 You:**
> "Is this sequence valid for an advanced user: exercise_01, exercise_05, exercise_02?"

**🤖 AI Agent:**
> No, the sequence is invalid because it skips essential intermediate movements required for advanced progression.


## ❓ FAQ

**Q: How do I generate a full session plan?**
You can use the `get_session_plan` tool by providing the client's proficiency level, the equipment being used, the session goals, and the desired duration.

**Q: Can I check if a sequence of exercises is safe for a beginner?**
Yes, use the `validate_progression_path` tool to verify if an exercise sequence follows a valid physiological progression for the specified client level.

**Q: What equipment is supported?**
The planner supports core GYROTONIC® apparatus such as the Pulley Tower and the Handle Unit. You can use `get_equipment_capabilities` to see specific exercises for each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gyrotonic-expansion-series-planner](https://vinkius.com/en/ai-agent-connect/gyrotonic-expansion-series-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GYROTONIC® Expansion Series Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gyrotonic-expansion-series-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GYROTONIC® Expansion Series Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gyrotonic-expansion-series-planner": {
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
