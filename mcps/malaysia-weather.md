# Malaysia Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/malaysia-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-services](../categories/data-services.md)

Get real-time tropical weather forecasts, severe weather warnings, and earthquake alerts for Malaysia and Southeast Asia from MET Malaysia.

## Description
The **Malaysia Weather MCP Server** provides direct, zero-auth access to the official Malaysian Meteorological Department (MET Malaysia) data feed — the authoritative source for tropical climate intelligence across the Malay Peninsula, Sabah, and Sarawak.

### Core Capabilities

- **7-Day Tropical Forecast** — Detailed morning, afternoon, and night weather predictions for every state, district, town, and recreation area in Malaysia. Temperature ranges included.
- **Severe Weather Warnings** — Active official alerts for heavy rain, strong winds, thunderstorms, and dangerous sea conditions. Bilingual content in English and Bahasa Melayu.
- **Earthquake Alerts** — Real-time seismic events detected in the Southeast Asian region, including distance measurements from the nearest Malaysian territory.
- **Automatic Translation** — All Malay-language forecast conditions are automatically translated to English for global accessibility.

Zero authentication required. Data sourced from MET Malaysia and updated daily. Essential for travel planners, logistics operators, insurance analysts, and anyone with operations in tropical Southeast Asia.


## Available Tools
- **get_malaysia_earthquakes**: Includes magnitude, depth, coordinates, and distance from nearest Malaysian location.

Get recent earthquake alerts reported by MET Malaysia for the Southeast Asian region
- **get_malaysia_forecast**: Forecasts include morning, afternoon, and night conditions with temperature ranges. You can filter by location name (e.g. Kuala Lumpur, Langkawi, Penang, Johor Bahru, Kota Kinabalu). All Malay forecast terms are automatically translated to English.

Get the 7-day weather forecast for locations across Malaysia
- **get_malaysia_warnings**: Bilingual content available in English and Bahasa Melayu.

Get active weather warnings issued by MET Malaysia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Malaysia Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather forecast for Kuala Lumpur this week?"

**🤖 AI Agent:**
> I've checked the MET Malaysia forecast for Kuala Lumpur. Expect isolated thunderstorms in the afternoon through Wednesday, with temperatures ranging from 25°C to 34°C. The mornings look clear with no rain expected.

---

**👤 You:**
> "Are there any earthquake alerts near Malaysia right now?"

**🤖 AI Agent:**
> I've checked the MET Malaysia seismic feed. The most recent event was a magnitude 5.5 earthquake in the Minahassa Peninsula, Sulawesi, at a depth of 135 km. It was located approximately 613 km southeast of Semporna, Sabah. The status is marked as NORMAL with no tsunami warning issued.


## ❓ FAQ

**Q: Do I need an API Key?**
No. The data.gov.my Weather API is completely open and requires zero authentication. For higher rate limits, an optional token can be requested via email to the Malaysian government.

**Q: Are the forecasts in English?**
The raw data from MET Malaysia uses Bahasa Melayu for forecast conditions. This server automatically translates all forecast terms to English, so you always receive clear, human-readable weather descriptions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/malaysia-weather](https://vinkius.com/mcp/malaysia-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Malaysia Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `malaysia-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Malaysia Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "malaysia-weather": {
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
