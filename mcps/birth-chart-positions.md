# Birth Chart Positions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/birth-chart-positions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate zodiac positions of celestial bodies based on date, time, and location.

## Description
This MCP server provides an astronomical calculation engine to translate a specific moment in time and geographic coordinates into a readable astrological map. Using simplified VSOP87 algorithms, it calculates the ecliptic longitude for the Sun, Moon, and all major planets (Mercury, Venus, Mars, Jupiter, Saturn, Uranus, Neptune, and Pluto). You can use `calculate_sky_map` to see where all bodies were located at a specific birth moment, `interpret_longitude` to convert raw degrees into zodiac signs, or `find_bodies_in_sign` to identify which planets occupy a particular sign.


## Available Tools (3)
- **calculate_sky_map**: Calculate planetary positions for a specific time and location
- **find_bodies_in_sign**: Find all planets currently in a specific zodiac sign
- **interpret_longitude**: Interpret ecliptic longitude into zodiac sign and degrees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Birth Chart Positions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were the planetary positions on July 15, 1995, at 14:30:00 UTC at latitude 40.7128 and longitude -74.0060?"

**🤖 AI Agent:**
> On July 15, 1995, the Sun was in Cancer (approx. 23°), the Moon was in Leo (approx. 12°), and Mars was in Libra (approx. 5°).

---

**👤 You:**
> "What zodiac sign does an ecliptic longitude of 145 degrees represent?"

**🤖 AI Agent:**
> An ecliptic longitude of 145 degrees corresponds to the sign of Leo, specifically at 15 degrees within the sign.

---

**👤 You:**
> "Which planets were located in the sign of Scorpio?"

**🤖 AI Agent:**
> The planets found in Scorpio were Saturn (at 12°) and Neptune (at 5°).


## ❓ FAQ

**Q: What information do I need to calculate a sky map?**
You need the date (YYYY-MM-DD), time (HH:mm:ss) in UTC, and the latitude and longitude of the location.

**Q: How accurate are these planetary positions?**
The engine uses a simplified version of the VSOP87 theory to provide approximate astronomical positions for the zodiacal mapping.

**Q: Can I find which planets are in Aries?**
Yes, you can use the `find_bodies_in_sign` tool and provide 'Aries' as the target sign name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/birth-chart-positions](https://vinkius.com/mcp/birth-chart-positions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Birth Chart Positions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `birth-chart-positions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Birth Chart Positions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "birth-chart-positions": {
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
