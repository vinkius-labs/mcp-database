# Planetary Hour Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planetary-hour-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the 24 planetary hours of a day and their ruling planets based on Chaldean tradition.

## Description
The Planetary Hour Calculator allows you to determine the exact timing and governing celestial body for each of the twenty-four planetary hours in a day. Based on ancient Chaldean astrology, it divides the daylight period (sunrise to sunset) and the nighttime period (sunset to next sunrise) into twelve equal segments each. Using tools like `get_planetary_schedule`, you can retrieve a full schedule including start times, end times, and the ruling planet for every hour. You can also use `calculate_segment_durations` to find the specific length of daytime and nighttime hours, or `get_day_planet_affinity` to identify which planet rules the first hour of a specific weekday.


## Available Tools (3)
- **get_day_planet_affinity**: Identify the primary ruler for the start of a specific weekday
- **get_planetary_schedule**: Generate a complete list of all twenty-four planetary hours for a specific day
- **calculate_segment_durations**: Determine the length of a single daylight and nighttime planetary hour


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planetary Hour Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the planetary schedule for today if sunrise is 06:00, sunset is 18:00, and next day sunrise is 06:00 on a Monday?"

**🤖 AI Agent:**
> The first hour starts at 06:00 with Moon. The daylight hours continue until 18:00, followed by nighttime hours starting at 18:00 and ending at 06:00 the next day.

---

**👤 You:**
> "How long is a single daytime planetary hour if sunrise is 05:30 and sunset is 19:30?"

**🤖 AI Agent:**
> A single daytime planetary hour lasts 80 minutes.

---

**👤 You:**
> "Which planet rules the first hour of a Friday?"

**🤖 AI Agent:**
> The planet ruling the first hour of Friday is Venus.


## ❓ FAQ

**Q: How are the planetary hours calculated?**
The daylight period from sunrise to sunset is divided into twelve equal segments, and the nighttime period from sunset to the next day's sunrise is also divided into twelve equal segments.

**Q: What is the Chaldean order used in this tool?**
The sequence follows the traditional order: Saturn, Jupiter, Mars, Sun, Venus, Mercury, and Moon.

**Q: Can I find out which planet rules a specific day?**
Yes, by using the `get_day_planet_affinity` tool, you can identify which planet governs the first hour of any given weekday.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planetary-hour-calculator](https://vinkius.com/mcp/planetary-hour-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Planetary Hour Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `planetary-hour-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Planetary Hour Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planetary-hour-calculator": {
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
