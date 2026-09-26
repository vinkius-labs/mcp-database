# Family Emergency Drill Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-emergency-drill-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured household emergency rehearsal schedules, roles, and checklists.

## Description
This MCP server helps households prepare for emergencies by generating structured rehearsal schedules. It uses rotation logic to ensure variety in scenarios like fire or flood. You can use `generate_drill_schedule` to create a timeline, `assign_drill_roles` to distribute tasks based on mobility needs and pets, `get_observation_checklist` for evaluation, and `get_debrief_prompts` to reflect on performance.


## Available Tools (4)
- **assign_drill_roles**: Assigns specific responsibilities to family members based on the scenario and their specific capabilities
- **generate_drill_schedule**: Creates a sequence of drills by applying rotation logic to the provided scenarios and availability
- **get_debrief_prompts**: Provides a set of reflective questions to be used by the household after the drill is completed
- **get_observation_checklist**: Generates a customized checklist to evaluate the execution of the drill


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Emergency Drill Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a monthly drill schedule for a family with fire and earthquake scenarios."

**🤖 AI Agent:**
> I have generated a monthly schedule rotating between fire and earthquake drills for your household.

---

**👤 You:**
> "Assign roles for a fire drill including a dog named Buddy."

**🤖 AI Agent:**
> Roles assigned: Alice as Leader, Bob as Pet Handler for Buddy, and Charlie as Supply Grabber.

---

**👤 You:**
> "Give me a checklist for an earthquake drill with mobility constraints."

**🤖 AI Agent:**
> Your checklist includes: Drop, Cover, and Hold On; checking assistance for mobility-impaired members; and verifying exit paths are clear.


## ❓ FAQ

**Q: How does the scheduling work?**
The `generate_drill_schedule` tool applies scenario rotation and ensures no two adjacent drills share more than one significant characteristic.

**Q: Can I account for pets in the drills?**
Yes, when using `assign_drill_roles`, you can include pet names to ensure specific roles are assigned for animal safety.

**Q: How are mobility needs handled?**
The system respects mobility constraints by ensuring individuals with needs are not assigned high-mobility roles like 'Sweeper'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-emergency-drill-planner](https://vinkius.com/en/ai-agent-connect/family-emergency-drill-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Emergency Drill Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-emergency-drill-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Emergency Drill Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-emergency-drill-planner": {
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
