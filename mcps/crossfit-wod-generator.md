# CrossFit WOD Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/crossfit-wod-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured CrossFit workouts based on time, equipment, and metabolic targets.

## Description
This MCP server provides a specialized engine for creating CrossFit-style Workouts of the Day (WOD). By connecting your AI client to Vinkius Edge, you can use tools like `generate_wod` to build complete workouts tailored to your available time, equipment, and skill level. It also includes `get_scaling_options` to adjust movements for any proficiency, `validate_equipment_suitability` to ensure you have the right gear, and `get_energy_system_guidelines` to target specific metabolic pathways like aerobic or anaerobic lactic systems.


## Available Tools (4)
- **generate_wod**: Ensure the user provides available time, equipment, skill level, and the target metabolic pathway.

Generates a complete CrossFit workout based on time, equipment, skill, and energy system
- **get_energy_system_guidelines**: Returns intensity and duration guidelines for a specific energy system
- **get_scaling_options**: Provides modifications for a specific movement to match a user's capability
- **validate_equipment_suitability**: Checks if a movement can be performed with the available equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrossFit WOD Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 15-minute CrossFit workout for an intermediate level using only dumbbells."

**🤖 AI Agent:**
> Workout Name: Dumbbell Burner. Structure: AMRAP 15 minutes. Exercises: 10 Dumbbell Thrusters, 15 Dumbbell Renegade Rows, 20 Dumbbell Goblet Squats. Target Stimulus: Anaerobic Lactic.

---

**👤 You:**
> "I'm a beginner. How can I scale a heavy barbell snatch?"

**🤖 AI Agent:**
> For a beginner, a primary scale for the snatch would be using dumbbells or kettlebells for a single-arm snatch to reduce technical complexity.

---

**👤 You:**
> "What are the guidelines for an aerobic energy system workout?"

**🤖 AI Agent:**
> Aerobic workouts typically involve steady-state work with a longer duration and a lower intensity to build cardiovascular endurance.


## ❓ FAQ

**Q: How do I create a workout?**
You can use the `generate_wod` tool by providing your available time, equipment list, skill level, and desired energy system target.

**Q: Can I adjust exercises if they are too difficult?**
Yes, use the `get_scaling_options` tool to receive specific modifications for any movement to match your skill level.

**Q: How do I know if I have the right equipment?**
The `validate_equipment_suitability` tool allows you to check if your current gear matches the requirements for specific movements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/crossfit-wod-generator](https://vinkius.com/en/ai-agent-connect/crossfit-wod-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrossFit WOD Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crossfit-wod-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrossFit WOD Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crossfit-wod-generator": {
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
