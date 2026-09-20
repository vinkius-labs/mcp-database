# GYROKINESIS® Session Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gyrokinesis-session-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates structured GYROKINESIS® exercise sessions based on level, focus, and time.

## Description
This MCP server acts as a specialized planning engine for GYROKINESIS® practitioners. It uses the unique GYROKINESIS® methodology to subdivide available time into structured phases: Warm-up, Main Exercise Sequences, Breath Work, and Cool-down. Users can utilize `get_session_plan` to generate a complete timed structure, `validate_equipment_compatibility` to ensure they have the necessary stool or mat for their focus areas, and `get_exercise_library_summary` to see available movement types. It adapts intensity and duration based on whether the user is at a Beginner, Intermediate, or Advanced level.


## Available Tools (4)
- **get_intensity_scaling_factors**: Retrieves the multipliers used to adjust phase durations based on the user's skill level
- **get_exercise_library_summary**: Provides a list of available exercise types filtered by equipment and focus
- **get_session_plan**: Generates a complete, timed GYROKINESIS® session structure
- **validate_equipment_compatibility**: Checks if the selected equipment is sufficient for the requested focus areas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GYROKINESIS® Session Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 30-minute Beginner GYROKINESIS® session focusing on the Spine with a stool."

**🤖 AI Agent:**
> Your 30-minute Beginner session is ready: 5 minutes of Warm-up, 15 minutes of Spinal Articulation sequences, 5 minutes of Breath Work, and 5 minutes of Cool-down.

---

**👤 You:**
> "I have 45 minutes and a mat. Plan an Intermediate session for Shoulders and Hips."

**🤖 AI Agent:**
> Your 45-minute Intermediate session is ready: 7 minutes of Warm-up, 25 minutes of Shoulder and Hip sequences, 5 minutes of Breath Work, and 8 minutes of Cool-down.

---

**👤 You:**
> "What exercises are available for a 20-minute session with no equipment?"

**🤖 AI Agent:**
> For a session with no equipment, you have access to Standing and Floor-based exercise categories.


## ❓ FAQ

**Q: How do I generate a full workout plan?**
You can use the `get_session_plan` tool by providing your class level, focus areas, available minutes, and equipment availability.

**Q: Do I need specific equipment for certain exercises?**
Yes. You can use `validate_equipment_compatibility` to check if your available equipment (like a stool or mat) matches your chosen focus areas.

**Q: Can I customize the session for my skill level?**
Yes, the session timing and intensity are automatically adjusted based on whether you select Beginner, Intermediate, or Advanced levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gyrokinesis-session-timer](https://vinkius.com/en/ai-agent-connect/gyrokinesis-session-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GYROKINESIS® Session Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gyrokinesis-session-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GYROKINESIS® Session Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gyrokinesis-session-timer": {
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
