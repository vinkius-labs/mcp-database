# AstrologyAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/astrologyapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Leading global astrology platform — get daily horoscopes, birth charts, and numerology via AI.

## Description
Empower your AI agent to orchestrate your celestial insights and astrological data with **AstrologyAPI**, the premier provider of global astrological calculations. By connecting AstrologyAPI to your agent, you transform complex birth chart generation, matchmaking analysis, and daily horoscope retrieval into a natural conversation. Your agent can instantly retrieve personalized predictions for any zodiac sign, calculate planetary positions based on birth metadata, and even generate numerology reports without you ever needing to navigate multiple spiritual apps or websites. Whether you are conducting a personal growth audit or coordinating spiritual wellness, your agent acts as a real-time astrological coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Celestial Orchestration** — Retrieve daily horoscopes covering personal, health, and career predictions for all zodiac signs.
- **Chart Auditing** — Calculate precise planetary and house positions based on date, time, and geographic coordinates.
- **Matchmaking Management** — Perform detailed compatibility analysis between individuals based on birth metadata.
- **Traditional Insights** — Access basic Panchang details and identify specialized planetary yogas.
- **Spiritual Monitoring** — Check Sade Sati status and generate comprehensive numerology reports using name and birth data.

### How it works

1. Subscribe to this server
2. Enter your AstrologyAPI.com User ID and API Key
3. Start managing your astrological data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Spiritual Researchers & Fans** — automate the gathering of daily predictions and celestial trends through natural language.
- **Wellness App Developers** — integrate professional-grade astrological calculations into your AI-driven routines.
- **Astrology Power Users** — integrate your existing spiritual data projects into your AI-driven daily routine to streamline your spiritual growth.


## Available Tools (8)
- **check_sade_sati**: Check Sade Sati status
- **get_ashtakvarga_score**: Calculate ashtakvarga points
- **get_basic_panchang**: Get daily panchang
- **get_daily_prediction**: Get daily horoscope
- **get_house_positions**: Get zodiac houses
- **get_matchmaking_details**: Analyze birth match
- **get_planets_positions**: Get birth chart planets
- **get_yoga_analysis**: Analyze planetary yogas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AstrologyAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the daily prediction for 'Scorpio'."

**🤖 AI Agent:**
> I've retrieved the daily prediction for Scorpio. Today, you should focus on personal communication and emotional balance. Your health outlook is stable, and there are positive trends in your career. Would you like me to check your numerology report for today as well?

---

**👤 You:**
> "Get the birth chart planets for: Born 12 Oct 1990, 14:30 in London (Lat: 51.5, Lon: -0.12, TZ: 1)."

**🤖 AI Agent:**
> I've calculated the planetary positions for that birth metadata. The Sun was in Libra, the Moon was in Cancer, and Mars was in Gemini. Should I also check the house positions or identify any specialized yogas in this chart?

---

**👤 You:**
> "Generate a numerology report for 'John Doe' born on 15 Jan 1985."

**🤖 AI Agent:**
> I've generated the numerology report for John Doe. Your Destiny Number is 3, reflecting creativity and self-expression. Your Radical Number is 6. Would you like me to provide a detailed explanation of what these numbers mean for your personal growth?


## ❓ FAQ

**Q: How do I find my AstrologyAPI User ID and Key?**
Log in to the [AstrologyAPI Dashboard](https://astrologyapi.com/), navigate to the 'API Settings' or 'My Account' section, and copy your unique User ID and API Key.

**Q: What is the coordinate format for birth charts?**
AstrologyAPI requires numeric Latitude and Longitude. For example, London is approximately `lat: 51.5` and `lon: -0.12`. You should also provide the correct timezone offset (e.g., `0` for London).

**Q: Does the API support Vedic astrology?**
Yes! AstrologyAPI is a leader in Vedic calculations. Tools like `get_basic_panchang` and `get_yoga_analysis` provide deep insights based on traditional Vedic principles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/astrologyapi](https://vinkius.com/mcp/astrologyapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AstrologyAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `astrologyapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AstrologyAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "astrologyapi": {
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
