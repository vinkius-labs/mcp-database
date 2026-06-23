# Business Timezone & Holiday Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/business-timezone-holiday-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Eradicate LLM scheduling errors. Calculate exact business days skipping global public holidays and convert precise timezones flawlessly.

## Description
LLMs hallucinate dates. They forget leap years, daylight saving time rules, and have no idea when Easter or local bank holidays occur. This MCP makes your AI a perfect executive assistant by giving it real-time calendar and holiday intelligence.

### Superpowers

- **Business Day Calculation:** Ask the AI for a 45-day SLA deadline. The MCP automatically skips weekends and fetches actual national public holidays (via the public Nager.Date API) for any country.
- **Flawless Timezones:** Instantly convert meeting times between complex IANA timezones (e.g., from `America/Sao_Paulo` to `Asia/Tokyo`), accounting for real-world offset rules.


## Available Tools (2)
- **add_business_days**: It automatically skips weekends. If you provide a countryCode (e.g. "US", "BR", "JP"), it will also query the Nager.Date API to skip national public holidays for that country.

Calculates a future date by adding a specific number of business days (skipping weekends and optional public holidays)
- **convert_timezone**: Uses IANA timezone strings (e.g. "America/Sao_Paulo", "Asia/Tokyo").

Converts an exact date and time from one timezone to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Timezone & Holiday Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I sign a contract in Brazil today (2026-05-15), what is the exact date 45 business days from now, skipping Brazilian holidays?"

**🤖 AI Agent:**
> I calculated 45 business days from 2026-05-15.

Skipping all weekends and public holidays in Brazil (BR), your deadline falls precisely on: **July 20, 2026**.

---

**👤 You:**
> "Convert our project launch time (October 15, 2026 at 14:30 in New York) to Tokyo time."

**🤖 AI Agent:**
> I converted the timezone.

**From (America/New_York):** October 15, 2026 at 2:30 PM
**To (Asia/Tokyo):** October 16, 2026 at 3:30 AM

Your launch in Tokyo will be early the next morning.


## ❓ FAQ

**Q: Does this require an API key?**
No. The timezone logic runs directly inside the Vinkius Edge process. For holiday lookups, it uses the free, public Nager.Date API without requiring authentication.

**Q: Why use this instead of letting the AI guess?**
AIs do not have access to live calendars or global holiday databases. They will frequently schedule your deadlines on a Sunday or a major national holiday. This MCP enforces absolute temporal accuracy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/business-timezone-holiday-scheduler](https://vinkius.com/mcp/business-timezone-holiday-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Timezone & Holiday Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-timezone-holiday-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Timezone & Holiday Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-timezone-holiday-scheduler": {
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
