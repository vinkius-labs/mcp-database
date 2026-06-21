# HUD User (USPS Crosswalk) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hud-user-usps-crosswalk)
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


## ❓ FAQ

**Q: How do I get a HUD User Access Token?**
Register for an account at the HUD User API page (https://www.huduser.gov/portal/dataset/uspszip-api.html), confirm your email, and generate a token in your user dashboard.

**Q: Which year of data is used?**
By default, the API returns the most recent available data. You can optionally specify a year and quarter in each tool.

**Q: Does it support mapping Tracts back to ZIP codes?**
Yes, tools like tract_to_zip and county_to_zip allow bidirectional crosswalking between geography IDs and ZIP codes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hud-user-usps-crosswalk](https://vinkius.com/mcp/hud-user-usps-crosswalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HUD User (USPS Crosswalk)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hud-user-usps-crosswalk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HUD User (USPS Crosswalk)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hud-user-usps-crosswalk": {
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
