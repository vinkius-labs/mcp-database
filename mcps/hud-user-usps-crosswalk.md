# HUD User (USPS Crosswalk) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hud-user-usps-crosswalk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hud-user-usps-crosswalk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hud-user-usps-crosswalk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Map ZIP codes to Census geographies via HUD User USPS Crosswalk API.

## Description
Empower your AI agents to navigate US geography with precision. This MCP server connects to the HUD User Data API to provide crosswalks between USPS ZIP codes and Census Bureau geographies including Tracts, Counties, CBSAs, and Congressional Districts. Essential for urban planning, demographics analysis, and real estate data processing.


## Available Tools
- **cbsa_to_zip**: Maps CBSAs to ZIP codes
- **cbsadiv_to_zip**: Maps CBSA Divisions to ZIP codes
- **cd_to_zip**: Maps Congressional Districts to ZIP codes
- **county_to_zip**: Maps Counties to ZIP codes
- **tract_to_zip**: Maps Census Tracts to ZIP codes
- **zip_to_cbsa**: Maps ZIP codes to Core Based Statistical Areas (CBSA)
- **zip_to_cbsadiv**: Maps ZIP codes to CBSA Divisions
- **zip_to_cd**: Maps ZIP codes to Congressional Districts
- **zip_to_county**: Maps ZIP codes to Counties
- **zip_to_tract**: Maps ZIP codes to Census Tracts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HUD User (USPS Crosswalk)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the census tracts associated with ZIP code 90210."

**🤖 AI Agent:**
> I'll retrieve the ZIP to Tract crosswalk for you.

---

**👤 You:**
> "Which ZIP codes are in county FIPS 06037?"

**🤖 AI Agent:**
> I'll map that county FIPS to its corresponding ZIP codes.

---

**👤 You:**
> "Get the congressional districts for ZIP code 10001."

**🤖 AI Agent:**
> I'll look up the congressional districts for that ZIP code.


## Installation & Usage

To install and use the **HUD User (USPS Crosswalk)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hud-user-usps-crosswalk](https://vinkius.com/mcp/hud-user-usps-crosswalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
