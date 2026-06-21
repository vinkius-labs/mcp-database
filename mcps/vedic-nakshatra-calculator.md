# Vedic Nakshatra Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vedic-nakshatra-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vedic-nakshatra-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vedic-nakshatra-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [astrology](../categories/astrology.md)

Determine precise lunar mansions (Nakshatras) and their astrological attributes.

## Description
The Vedic Nakshatra Calculator provides precise astronomical computations to identify the Moon's position within the 27 lunar mansions. By using tools like `get_nakshatra_details`, you can uncover the ruling deity, symbol, and guna (quality) of a specific moment in time based on birth coordinates. The server also allows for raw data retrieval via `calculate_lunar_position` to understand ecliptic longitude and ayanamsa adjustments, or viewing the full zodiac inventory with `list_all_constellations`.


## Available Tools
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


## Installation & Usage

To install and use the **Vedic Nakshatra Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vedic-nakshatra-calculator](https://vinkius.com/mcp/vedic-nakshatra-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
