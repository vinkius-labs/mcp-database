# Surf Interval Trainer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-interval-trainer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Optimized interval training protocols designed specifically for surf fitness and paddle endurance.

## Description
This MCP server provides specialized interval training design for surfers. It calculates optimal work/rest ratios and session structures to improve anaerobic power and aerobic capacity. Use `plan_session` to generate a complete workout, `calculate_ratios` to find ideal timing for your goals, or `get_interval_presets` to see available templates. It also includes `validate_session_feasibility` to ensure your training remains safe and effective based on your current fitness tier.


## Available Tools (4)
- **calculate_ratios**: Determines the optimal work-to-rest time relationship for a specific goal and fitness level
- **get_interval_presets**: Provides a list of standardized interval templates available for the user
- **plan_session**: Generates a complete, structured interval training session based on user profile and constraints
- **validate_session_feasibility**: Checks if a proposed workout structure is safe and effective for a specific user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Interval Trainer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 20 minute surf fitness session for an Intermediate level aiming for AnaerobicPower."

**🤖 AI Agent:**
> Your 20-minute AnaerobicPower session is ready. It includes a 5-minute warm-up, 10 sets of 30-second high-intensity bursts followed by 60 seconds of rest, and a 5-minute cool-down.

---

**👤 You:**
> "What are the best work/rest ratios for a Beginner looking to build AerobicBase?"

**🤖 AI Agent:**
> For a Beginner focusing on AerobicBase, the recommended ratio is 30 seconds of work followed by 90 seconds of rest.

---

**👤 You:**
> "Show me the available training presets for an Advanced surfer."

**🤖 AI Agent:**
> Available presets for Advanced level: 'Explosive Sprint' (15s work/45s rest), 'Endurance Builder' (60s work/30s rest), and 'Power Intervals' (30s work/30s rest).


## ❓ FAQ

**Q: How do I generate a full workout?**
You can use the `plan_session` tool by providing your fitness level, target goal, and available time.

**Q: Can I check if a workout is safe for me?**
Yes, use `validate_session_feasibility` to verify if your planned work and rest durations are appropriate for your fitness level.

**Q: What training goals are supported?**
The server supports AerobicBase, AnaerobicPower, and MuscularEndurance goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-interval-trainer](https://vinkius.com/en/ai-agent-connect/surf-interval-trainer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Interval Trainer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-interval-trainer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Interval Trainer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-interval-trainer": {
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
