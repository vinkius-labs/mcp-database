# Vedic Nakshatra Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vedic-nakshatra-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [astrology](../categories/astrology.md)

Determine precise lunar mansions (Nakshatras) and their astrological attributes.

## Description
The Vedic Nakshatra Calculator provides precise astronomical computations to identify the Moon's position within the 27 lunar mansions. By using tools like `get_nakshatra_details`, you can uncover the ruling deity, symbol, and guna (quality) of a specific moment in time based on birth coordinates. The server also allows for raw data retrieval via `calculate_lunar_position` to understand ecliptic longitude and ayanamsa adjustments, or viewing the full zodiac inventory with `list_all_constellations`.


## Available Tools (3)
- **calculate_lunar_position**: Provides the raw astronomical longitude used for astrological computations
- **get_nakshatra_details**: Identifies the specific Nakshatra and all its associated attributes for a given moment in time
- **list_all_constellations**: Provides a complete inventory of all 27 Nakshatras and their primary identifiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vedic Nakshatra Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the Nakshatra for someone born on 1990-05-15 at 10:30 in New York (Lat: 40.71, Lon: -74.00)."

**🤖 AI Agent:**
> The tool `get_nakshatra_details` would return the specific Nakshatra name, its ruling deity, symbol, and the calculated pada.

---

**👤 You:**
> "List all the constellations in the zodiac."

**🤖 AI Agent:**
> Using `list_all_constellations`, the tool returns a complete list of all 27 Nakshatras with their respective symbols.

---

**👤 You:**
> "What is the lunar longitude for 2023-10-01 at 12:00 in London?"

**🤖 AI Agent:**
> The `calculate_lunar_position` tool will provide the ecliptic longitude and the ayanamsa value for that specific time.


## ❓ FAQ

**Q: What is a Nakshatra?**
A Nakshatra is one of the 27 lunar mansions in Vedic astrology, representing a specific segment of the ecliptic path of the Moon.

**Q: How accurate are the calculations?**
The tool uses precise astronomical algorithms to calculate the Moon's ecliptic longitude and applies the necessary Ayanamsa correction for sidereal zodiac accuracy.

**Q: Can I use this for any date and time?**
Yes, as long as you provide a valid ISO 8601 date and time along with the correct geographic coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vedic-nakshatra-calculator](https://vinkius.com/mcp/vedic-nakshatra-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vedic Nakshatra Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vedic-nakshatra-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vedic Nakshatra Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vedic-nakshatra-calculator": {
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
