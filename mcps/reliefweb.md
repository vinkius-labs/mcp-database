# ReliefWeb MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reliefweb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reliefweb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reliefweb-mcp)
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


## Available Tools
- **get_countries**: Returns country names, ISO codes and associated disaster counts. Useful for finding country IDs to use in report searches.

Search countries in the ReliefWeb database
- **get_disasters**: Returns disaster names, types (earthquake, flood, cyclone, etc.), start dates and affected countries.

Search disasters (earthquakes, floods, cyclones, etc.)
- **get_formats**: Returns format names and IDs (Situation Report, Assessment, Press Release, Map, etc.) for filtering reports by type.

Get report formats
- **get_jobs**: Returns job titles, organizations, locations, types and posting dates.

Search humanitarian job postings
- **get_organizations**: Returns organization names, types and report counts.

Search humanitarian organizations
- **get_report**: Returns full report metadata including title, body, source, themes, countries, disasters and file attachments.

Get a specific report by ID
- **get_reports**: Supports free-text query, date range filtering, and filtering by country, disaster type, theme, format, source, organization and language. Returns report titles, dates, sources, themes and links.

Search humanitarian reports
- **get_sources**: Returns source names and types.

Get report sources
- **get_themes**: Returns theme names and IDs for filtering reports by topic (Health, Shelter, Food, Protection, etc.).

Get report themes


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


## Installation & Usage

To install and use the **ReliefWeb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reliefweb](https://vinkius.com/mcp/reliefweb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
