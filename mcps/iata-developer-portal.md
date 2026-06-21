# IATA Developer Portal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iata-developer-portal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iata-developer-portal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iata-developer-portal-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access aviation reference data — audit airports, airlines, and aircraft via AI.

## Description
Empower your AI agent to orchestrate your entire aviation research and logistics auditing workflow with the **IATA Developer Portal**, the official source for global aviation standards. By connecting IATA's reference data to your agent, you transform complex industry searches into a natural conversation. Your agent can instantly search for airport codes, audit airline identifiers, and retrieve aircraft metadata without you ever touching a technical manual. Whether you are conducting logistics research or building travel applications, your agent acts as a real-time aviation consultant, ensuring your data is always grounded in official, IATA-verified standards.

### What you can do

- **Airport Auditing** — Search for global airports by IATA code and retrieve detailed metadata, including names and geographic locations.
- **Airline Oversight** — Audit airline identifiers and codes to maintain a clear view of carrier distribution and names.
- **Aircraft Intelligence** — Query aircraft types and codes to understand the technical equipment used in global logistics.
- **City Discovery** — Retrieve detailed city information associated with specific IATA codes to assist in geographic planning.
- **Global Monitoring** — List all supported countries in the IATA catalog to maintain strict organizational control over regional data.

### How it works

1. Subscribe to this server
2. Enter your IATA API Key
3. Start managing your aviation intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Planners** — monitor aviation codes and retrieve airport metadata straight from your workflow.
- **Travel Developers** — verify airline identifiers and audit aircraft types without manual searching.
- **Aviation Researchers** — perform rapid audits of global aviation standards and codes through natural language.
- **Operations Leads** — automate aviation data querying to orchestrate cross-functional logistics teams smoothly.


## Available Tools
- **check_api_status**: Check if the IATA API is operational
- **get_city_details**: Get details for a specific city by IATA city code
- **search_airlines**: Search for airlines by IATA code
- **list_iata_countries**: List all countries supported by IATA
- **search_aircraft**: Search for aircraft by IATA code
- **search_airports**: Search for airports by IATA code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IATA Developer Portal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for airport with IATA code 'LHR' (London Heathrow) using IATA Portal."

**🤖 AI Agent:**
> I've retrieved the details for London Heathrow Airport. It is located in the United Kingdom and uses timezone Europe/London. Would you like the full geographic coordinates or city metadata?

---

**👤 You:**
> "Identify the airline with code 'BA' (British Airways)."

**🤖 AI Agent:**
> I've identified the airline as British Airways. I can retrieve the full name and operational metadata for this carrier if you'd like.

---

**👤 You:**
> "What aircraft corresponds to IATA code '744'?"

**🤖 AI Agent:**
> I've retrieved the details. The IATA code '744' corresponds to the Boeing 747-400 (Passenger) aircraft. I can assist you with more aircraft metadata if needed.


## Installation & Usage

To install and use the **IATA Developer Portal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iata-developer-portal](https://vinkius.com/mcp/iata-developer-portal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
