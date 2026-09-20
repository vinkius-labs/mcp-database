# Percussive Therapy Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/percussive-therapy-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Plan optimal massage gun sessions with precise speed and duration settings.

## Description
This MCP server provides specialized session planning for percussive massage devices. It calculates optimal speed settings, pressure levels, and treatment durations for specific muscle groups based on your treatment goals and sensitivity. Use `get_session_plan` to generate a full schedule or `get_speed_recommendation` to find the best frequency for your device.


## Available Tools (4)
- **calculate_area_duration**: Determines how many seconds a specific muscle should be treated
- **get_session_plan**: Generates a comprehensive percussion session schedule based on user needs
- **get_speed_recommendation**: Provides the optimal device frequency for a specific goal and sensitivity profile
- **validate_muscle_group**: Verifies if a requested muscle group is supported by the application's guidelines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percussive Therapy Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a recovery session for my glutes and calves. My device goes from 1200 to 3200 RPM, and I have medium sensitivity."

**🤖 AI Agent:**
> Your recovery session is ready. For the glutes, use speed 1800 RPM for 90 seconds. For the calves, use speed 1600 RPM for 60 seconds. Total session time: 2.5 minutes.

---

**👤 You:**
> "What is the best speed for deep tissue work on my quads if I have low sensitivity? My device range is 1000-3000 RPM."

**🤖 AI Agent:**
> For deep tissue work on your quads with low sensitivity, the recommended speed is 2400 RPM.

---

**👤 You:**
> "How long should I treat my hamstrings for a maintenance goal?"

**🤖 AI Agent:**
> For a maintenance goal, you should treat your hamstrings for 75 seconds.


## ❓ FAQ

**Q: How do I create a full session plan?**
You can use the `get_session_plan` tool by providing the muscle groups you want to treat, your goal, sensitivity, and your device's speed range.

**Q: Can I check if a specific muscle is supported?**
Yes, use the `validate_muscle_group` tool to verify if a requested anatomical area is included in the therapy guidelines.

**Q: How is the speed setting determined?**
The speed is calculated by balancing your treatment goal with your personal sensitivity and the limits of your device using `get_speed_recommendation`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/percussive-therapy-timer](https://vinkius.com/en/ai-agent-connect/percussive-therapy-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Percussive Therapy Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `percussive-therapy-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Percussive Therapy Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "percussive-therapy-timer": {
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
