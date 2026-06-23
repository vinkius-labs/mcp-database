# IPGeolocation (IP Intelligence & Time) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipgeolocation-ip-intelligence-time)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Resolve IP addresses via IPGeolocation — get precise location, timezone details, and local astronomy data.

## Description
Connect your **IPGeolocation.io** account to any AI agent and take full control of global IP intelligence and time-based analytics through natural conversation.

### What you can do

- **IP Intelligence** — Resolve IPv4 or IPv6 addresses to precise geographic locations, including city, country, and GPS coordinates directly from your agent
- **Network Audit** — Extract detailed ISP information, organization names, and connection types to identify the infrastructure behind any IP request
- **Timezone Analytics** — Retrieve precise local time, UTC offsets, and Daylight Saving Time (DST) status for any global location or coordinate set
- **Astronomy Data** — Access planetary metrics including sunrise, sunset, and moon phases for specific Earth locations to power context-aware applications
- **Financial Localization** — Get local currency details, including names and symbols, associated with an IP's detected jurisdiction for localized pricing audits
- **Geo-Spatial Tools** — Perform location and astronomy lookups using direct latitude and longitude coordinates when an IP address is not available

### How it works

1. Subscribe to this server
2. Enter your IPGeolocation API Key
3. Start resolving global intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — automate the localization of user experiences and validate time-based application logic through natural conversation
- **Security Analysts** — identify the geographic origin and ISP details of suspicious IP addresses for rapid incident response
- **Data Engineers** — enrich server logs and visitor datasets with precise geolocation and astronomical metadata efficiently


## Available Tools (3)
- **get_location**: Retrieve comprehensive geolocation data for an IP address
- **get_timezone**: Get precise local time and timezone information
- **get_astronomy**: Retrieve astronomy data like sunrise and moon phases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPGeolocation (IP Intelligence & Time)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve the location for IP address '8.8.8.8'"

**🤖 AI Agent:**
> Resolving IP '8.8.8.8'… This address is located in Mountain View, California, United States. It belongs to the 'Google LLC' ISP. GPS Coordinates: 37.4223, -122.0841. Local currency is USD ($).

---

**👤 You:**
> "What is the current local time and UTC offset in Tokyo?"

**🤖 AI Agent:**
> Current local time in Tokyo (Asia/Tokyo) is 10:45 PM (Tuesday). The UTC offset is +09:00. Daylight Saving Time is currently not active in this region.

---

**👤 You:**
> "Show me the sunrise and sunset times for Lisbon today"

**🤖 AI Agent:**
> Retrieving astronomy data for Lisbon… Today, the sun rises at 7:12 AM and sets at 6:45 PM. The solar noon occurs at 12:58 PM, and the total day length will be 11 hours and 33 minutes.


## ❓ FAQ

**Q: Can I resolve a location using GPS coordinates instead of an IP address?**
Yes. Tools like `get_timezone` and `get_astronomy` accept optional latitude and longitude parameters. This allows your agent to retrieve environmental and temporal data for any point on Earth, even if you don't have a target IP.

**Q: How do I check if a specific location is currently observed in Daylight Saving Time (DST)?**
Use the `get_timezone` tool by providing a timezone name (e.g. 'America/New_York'). Your agent will return the full timezone payload, including the `is_dst` boolean and current UTC offset.

**Q: Can my agent find out the sunrise and sunset times for a given IP?**
Absolutely. Use the `get_astronomy` tool and provide the target IP. Your agent will calculate the precise location and return astronomical data including sunrise, sunset, solar noon, and day length.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipgeolocation-ip-intelligence-time](https://vinkius.com/mcp/ipgeolocation-ip-intelligence-time)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IPGeolocation (IP Intelligence & Time)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipgeolocation-ip-intelligence-time` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPGeolocation (IP Intelligence & Time)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipgeolocation-ip-intelligence-time": {
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
