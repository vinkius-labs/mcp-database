# Western Astrology Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/western-astrology-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate sun signs, moon signs, ascendants, and planetary positions.

## Description
This MCP server provides deterministic astrological calculations for the tropical zodiac. It allows AI agents to determine a user's sun sign using `get_sun_sign`, approximate the moon sign via `get_moon_sign`, and calculate the rising sign (ascendant) using `get_ascendant`. Additionally, it provides estimated planetary positions through `get_planetary_positions` and calculates house cusps using a simplified Placidus system with `get_house_cusps`.


## Available Tools (5)
- **get_planetary_positions**: Estimates the zodiac positions of major planets
- **get_ascendant**: Calculates the Rising Sign (Ascendant) for a specific birth moment and location
- **get_house_cusps**: Calculates the starting points (cusps) of the twelve houses
- **get_moon_sign**: Provides an approximation of the Moon's zodiac placement
- **get_sun_sign**: Determines the primary zodiac sign based on the user's birth date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Western Astrology Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my sun sign if I was born on 1990-05-15?"

**🤖 AI Agent:**
> Your sun sign is Taurus.

---

**👤 You:**
> "What was my rising sign on 1990-05-15 at 14:30 in London (latitude 51.5, longitude -0.12)?"

**🤖 AI Agent:**
> Your rising sign is Leo.

---

**👤 You:**
> "Where were the planets located on 1990-05-15?"

**🤖 AI Agent:**
> On May 15, 1990, Mars was in Taurus, Jupiter was in Cancer, and Saturn was in Capricorn.


## ❓ FAQ

**Q: How accurate are the planetary positions?**
Planetary positions are estimated using mean orbital elements with an accuracy of approximately ±2 degrees.

**Q: What is the difference between the sun sign and the ascendant?**
The sun sign is determined by your birth date, while the ascendant is the sign rising on the eastern horizon at your specific birth time and location.

**Q: Can I use this with Claude or Cursor?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/western-astrology-calculator](https://vinkius.com/ai-agent-connect/western-astrology-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Western Astrology Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `western-astrology-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Western Astrology Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "western-astrology-calculator": {
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
