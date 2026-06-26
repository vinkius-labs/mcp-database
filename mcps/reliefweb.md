# ReliefWeb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reliefweb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access humanitarian reports, disaster data, job postings and organizational data from the world's leading humanitarian information platform.

## Description
Connect to **ReliefWeb** and explore the world's largest humanitarian information database through natural conversation — no API key needed.

### What you can do

- **Report Search** — Search humanitarian reports, situation updates and assessments with filters for country, disaster, theme, format, organization and date range
- **Disaster Data** — Browse tracked disasters including earthquakes, floods, cyclones, droughts and conflicts
- **Countries** — Get country information and associated humanitarian data
- **Organizations** — Find UN agencies, NGOs and government bodies publishing humanitarian data
- **Job Postings** — Search humanitarian job opportunities worldwide
- **Themes & Formats** — Explore report categories (Health, Shelter, Food, Protection) and formats (Situation Report, Assessment, Map)

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore humanitarian data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Humanitarian Workers** — find situation reports, assessments and operational guidance for crisis response
- **Researchers** — access structured humanitarian data for analysis and trend identification
- **Journalists** — discover reports, sources and organizational data for crisis coverage


## Available Tools (7)
- **get_countries**: Returns country names, ISO codes and status. Useful for finding country references to use in report or disaster searches.

Search countries in the ReliefWeb database
- **get_disasters**: Returns disaster names, types (Earthquake, Flood, Cyclone, etc.), dates and affected countries.

Search disasters (earthquakes, floods, cyclones, etc.)
- **get_jobs**: Returns job titles, organizations, locations, career categories and posting dates.

Search humanitarian job postings
- **get_report**: Returns full report metadata including title, body, source, themes, countries, disasters and file attachments.

Get a specific report by ID
- **get_reports**: Supports free-text query, date range filtering, and filtering by country, disaster type, theme, format, source and language. Returns report titles, dates, sources, themes and links.

Search humanitarian reports
- **get_sources**: Returns organization names, shortnames, types and countries. Covers UN agencies, NGOs, governments and academic institutions.

Search humanitarian organizations and sources
- **get_training**: Returns training titles, providers, locations, themes and registration dates.

Search humanitarian training opportunities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ReliefWeb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find situation reports about earthquakes in Turkey."

**🤖 AI Agent:**
> Found 45+ reports about earthquakes in Turkey. Recent situation reports from UN OCHA, IFRC and local organizations include damage assessments, casualty figures and humanitarian response updates.

---

**👤 You:**
> "What disasters are currently active?"

**🤖 AI Agent:**
> Currently tracked disasters: Cyclone Freddy (Mozambique/Malawi, orange alert), Earthquake M6.8 (Japan), Floods (Kenya), Drought (Horn of Africa). Each with affected population estimates and response status.

---

**👤 You:**
> "Show me humanitarian job postings in South Sudan."

**🤖 AI Agent:**
> Found 12 humanitarian jobs in South Sudan: WASH Coordinator (Save the Children), Health Manager (MSF), Protection Officer (UNHCR), Logistics Coordinator (WFP). All with application deadlines and organization details.


## ❓ FAQ

**Q: Do I need an API key?**
No! ReliefWeb's API is completely free and open. No authentication required. Just subscribe and start searching. Data is updated continuously.

**Q: What kind of reports are available?**
ReliefWeb hosts 300,000+ reports including situation reports, assessments, press releases, maps, infographics and evaluations from UN agencies, NGOs, governments and research organizations.

**Q: Can I search reports by country?**
Yes! Use get_reports with the country parameter to filter reports by country name. You can also filter by disaster type, theme, format, date range and organization simultaneously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reliefweb](https://vinkius.com/mcp/reliefweb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ReliefWeb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reliefweb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ReliefWeb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reliefweb": {
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
