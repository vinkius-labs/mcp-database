# WHO Athena API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/who-athena-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/who-athena-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/who-athena-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global health data — audit indicators and trends via AI.

## Description
Empower your AI agent to orchestrate your entire public health research and policy auditing workflow with the **WHO Athena API**, the authoritative source for global health indicators from the World Health Organization. By connecting the WHO GHO service to your agent, you transform complex medical searches into a natural conversation. Your agent can instantly retrieve historical datasets, audit regional health trends, and query specific indicator codes without you ever touching a health portal. Whether you are conducting epidemiological research or managing regional policy constraints, your agent acts as a real-time health analyst, ensuring your intelligence is always verified and precise.

### What you can do

- **Indicator Auditing** — Retrieve high-resolution statistical data for thousands of WHO health identifiers and maintain a clear view of global health changes.
- **Trend Oversight** — Audit historical health statistics to understand the longitudinal distribution of medical scale instantly.
- **Dimension Discovery** — Browse all available observation dimensions like 'country' or 'year' to maintain strict organizational control over your research.
- **Medical Intelligence** — Retrieve unique indicator codes and observation metadata to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your health research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (WHO GHO API is a free and open service)
3. Start managing your health intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health Analysts & Policy Makers** — monitor global trends and retrieve official metadata straight from your workflow.
- **Epidemiologists & Researchers** — verify statistical data and audit series patterns without manual searching.
- **Medical Journalists** — perform rapid audits of regional indicators and identify relevant health patterns through natural language.
- **Operations Leads** — automate health data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **get_health_indicator_data**: Get data for a specific WHO health indicator code
- **list_health_dimensions**: List all observation dimensions (e.g., country, year) available
- **list_health_indicators**: List all health indicators available in the WHO GHO database
- **check_api_status**: Check if the WHO GHO Athena service is operational


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHO Athena API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get data for 'Life expectancy at birth' (WHOSIS_000001) using WHO Athena."

**🤖 AI Agent:**
> I've retrieved the data for life expectancy! The latest observations show a global average of [Value] years. I can provide the breakdown by country or region metadata for you.

---

**👤 You:**
> "List all health indicators available in the WHO catalog."

**🤖 AI Agent:**
> I've scanned the WHO indicator catalog! There are thousands of series available, including markers for infectious diseases, child mortality, and health systems. I can help you find a specific code for your research.

---

**👤 You:**
> "What are the latest observations for 'Child mortality rate'?"

**🤖 AI Agent:**
> I've retrieved the observations for child mortality! The recent data points indicate a trend of [Value] per 1000 live births. I can assist you with an audit of the comparative metadata across different WHO regions if you'd like.


## Installation & Usage

To install and use the **WHO Athena API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/who-athena-api](https://vinkius.com/mcp/who-athena-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
