# Energy Curve Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/energy-curve-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Map your natural energy peaks, valleys, and optimal focus windows based on your chronotype.

## Description
The Energy Curve Mapper connects your biological rhythm to your daily schedule. By providing your chronotype (lion, bear, wolf, or dolphin) and your wake-up time, you can use tools like `get_daily_energy_map` to see a full 2-hour chronological sequence of your energy states. You can also specifically extract periods for deep work using `identify_focus_windows`, find ideal brainstorming times with `detect_creativity_windows`, or check your immediate biological state with `get_current_energy_status`.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Energy Curve Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my energy map for a bear chronotype who woke up at 08:00."

**🤖 AI Agent:**
> [{"startTime": "08:00", "endTime": "11:00", "energyState": "focus"}, {"startTime": "11:00", "endime": "14:00", "energyState": "peak"}, {"startTime": "14:00", "endTime": "17:00", "energyState": "creativity"}, {"startTime": "17:00", "endTime": "20:00", "energyState": "valley"}]

---

**👤 You:**
> "When are my focus windows if I am a lion and woke up at 06:00?"

**🤖 AI Agent:**
> [{"start": "06:00", "end": "08:00"}, {"start": "08:00", "end": "10:00"}]

---

**👤 You:**
> "What is my current energy state? I am a wolf, woke up at 10:00, and it is now 22:00."

**🤖 AI Agent:**
> Your current energy state is peak.


## ❓ FAQ

**Q: What is a chronotype?**
A chronotype is your natural biological inclination towards being awake or asleep at certain times of the day, such as 'lion' for early risers or 'wolf' for night owls. Tools available: `your_tool_name`.

**Q: How can I find my focus windows?**
You can use the `identify_focus_windows` tool by providing your chronotype and wake-up time to see when you are most capable of deep, concentrated work.

**Q: Does this tool work with any wake-up time?**
Yes, as long as you provide the time in a valid 24-hour format (e.g., '07:30').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/energy-curve-mapper](https://vinkius.com/mcp/energy-curve-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Energy Curve Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `energy-curve-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Energy Curve Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "energy-curve-mapper": {
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
