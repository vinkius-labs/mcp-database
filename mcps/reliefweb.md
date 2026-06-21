# ReliefWeb MCP Server

Access humanitarian reports, disaster data, job postings and organizational data from the world's leading humanitarian information platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reliefweb)

## Overview
**Category:** knowledge-management
**Tools Count:** 9

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


## Installation & Usage

To install and use the **ReliefWeb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reliefweb](https://vinkius.com/mcp/reliefweb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
