# BreezoMeter Air Quality & Pollen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/breezometer-air-quality-pollen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Universal air quality intelligence — get real-time AQI, pollutants, and pollen data via AI.

## Description
Equip your AI agent with hyper-local environmental intelligence through the **BreezoMeter** MCP server. This integration provides real-time access to accurate air quality and pollen data for any coordinate on Earth. Your agent can retrieve the BreezoMeter Air Quality Index (BAQI), identify dominant pollutants (PM2.5, NO2, etc.), and provide actionable health recommendations for sensitive groups. It also tracks pollen levels from various plants and trees to help users manage allergies. Whether you are building a health-tracking app, planning outdoor activities, or researching urban pollution, your agent acts as a dedicated environmental consultant through natural conversation.

### What you can do

- **Real-time Air Quality** — Get the current AQI and pollutant concentrations for any latitude/longitude.
- **Pollen Tracking** — Monitor pollen levels for specific tree, grass, and weed types.
- **Health Recommendations** — Access tailored advice for children, athletes, and individuals with respiratory conditions.
- **Global Coverage** — Retrieve environmental data for any street-level location worldwide.

### How it works

1. Subscribe to this server
2. Enter your BreezoMeter API Key (get it at breezometer.com)
3. Start monitoring air quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health & Wellness Enthusiasts** — monitor air quality to plan outdoor exercise and protect their health.
- **Allergy Sufferers** — track pollen counts to manage symptoms and plan their day.
- **Smart City Developers** — integrate environmental data into urban planning and monitoring tools.
- **Operations Managers** — verify local conditions for outdoor work and site safety.


## Available Tools (2)
- **get_air_quality**: Get current air quality for a location
- **get_pollen_levels**: Get current pollen data for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BreezoMeter Air Quality & Pollen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the air quality in New York right now?"

**🤖 AI Agent:**
> Retrieving air quality for New York... The current BAQI score is 72, which is 'Good'. The dominant pollutant is PM2.5. I also have health recommendations for outdoor activities. Would you like to see them?

---

**👤 You:**
> "Check the pollen risk in Berlin today."

**🤖 AI Agent:**
> I've fetched the pollen data for Berlin. Currently, grass pollen is at a 'Moderate' risk level, while tree pollen remains 'Low'. I can provide a more detailed breakdown if needed.

---

**👤 You:**
> "Are there any health warnings for sensitive groups in London?"

**🤖 AI Agent:**
> Analyzing London's environment... The AQI is currently 45. For sensitive groups (like those with asthma), it is recommended to limit prolonged outdoor exertion today. Would you like to see the specific pollutants causing this?


## ❓ FAQ

**Q: Can I check the pollen count in Paris?**
Yes! Use the `get_pollen_levels` tool and provide the latitude and longitude for Paris. It will return the current risk levels for various types of pollen.

**Q: What does the BAQI score represent?**
BAQI stands for BreezoMeter Air Quality Index. It is a standardized scale from 0 to 100, where 100 is excellent air quality and 0 is very poor.

**Q: Does it provide health advice for athletes?**
Yes. The health recommendations include specific advice for outdoor sports and physical activities based on the current pollutant levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/breezometer-air-quality-pollen](https://vinkius.com/mcp/breezometer-air-quality-pollen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BreezoMeter Air Quality & Pollen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breezometer-air-quality-pollen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BreezoMeter Air Quality & Pollen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breezometer-air-quality-pollen": {
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
