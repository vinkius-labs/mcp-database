# FRED Releases — Economic Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-releases-economic-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Track every U.S. economic data release: Employment Situation, GDP Advance, CPI, Federal Funds Rate, and hundreds more — with release schedules, historical dates, and the complete series within each release.

## Description
Never miss an economic data release again. FRED Releases gives your AI agent real-time awareness of the U.S. economic calendar.

### What you can do
- **Browse All Releases** — Employment Situation (BLS), GDP (BEA), CPI, PPI, FOMC, and 300+ official releases
- **Release Dates** — Upcoming and historical release dates — build your own economic calendar
- **Series Discovery** — Find all series within a release (e.g., release 10 has UNRATE, PAYEMS, and 500+ series)

### Key Release IDs
`10` Employment Situation · `53` GDP · `46` CPI · `21` Federal Funds Rate · `189` Housing Starts

### Who is this for?
Traders, fund managers, economic journalists, central bank watchers, and macro strategists who need to track when critical economic data drops.


## Available Tools (4)
- **list_releases**: Each release contains multiple series.

List all FRED economic data releases
- **get_release**: Use release IDs like 10 (Employment Situation), 53 (GDP), 46 (CPI).

Get details for a specific FRED release
- **get_release_dates**: Without release_id, returns dates for all releases (great for economic calendar). With release_id, returns dates for a specific release.

Get release dates for economic data
- **get_release_series**: For example, release 10 (Employment Situation) contains UNRATE, PAYEMS, and hundreds more.

Get all series within a FRED release


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FRED Releases — Economic Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is the next Employment Situation release?"

**🤖 AI Agent:**
> 📅 **Employment Situation (Release #10)**

Next release: February 7, 2025 (8:30 AM ET)
Previous: January 10, 2025
Source: Bureau of Labor Statistics (BLS)

This release contains UNRATE, PAYEMS, and 500+ employment series.

---

**👤 You:**
> "What series are included in the GDP release?"

**🤖 AI Agent:**
> 💰 **GDP Release (#53) — Key Series**

- GDP — Gross Domestic Product
- GDPC1 — Real GDP (Chained 2017 Dollars)
- A191RL1Q225SBEA — Real GDP % Change
- PCEC — Personal Consumption
- GPDI — Gross Private Domestic Investment

+200 more series in this release.

---

**👤 You:**
> "Show me the upcoming economic calendar for this week"

**🤖 AI Agent:**
> 📅 **This Week — Economic Releases**

| Date | Release | Source |
|------|---------|--------|
| Mon | ISM Manufacturing | ISM |
| Tue | JOLTS Job Openings | BLS |
| Wed | ADP Employment | ADP |
| Thu | Initial Claims | DOL |
| Fri | Employment Situation | BLS |

The Jobs Report (Friday) is the market-moving headline event.


## ❓ FAQ

**Q: What is a FRED release?**
A release is a collection of related series published together on a schedule. For example, the 'Employment Situation' release (#10) published monthly by BLS contains unemployment rate, nonfarm payrolls, and 500+ labor market series.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-releases-economic-calendar](https://vinkius.com/mcp/fred-releases-economic-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FRED Releases — Economic Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fred-releases-economic-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FRED Releases — Economic Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fred-releases-economic-calendar": {
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
