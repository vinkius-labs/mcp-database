# Ayuntamiento de Zaragoza MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ayuntamiento-de-zaragoza)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ayuntamiento-de-zaragoza-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ayuntamiento-de-zaragoza-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access Zaragoza's open data, city services (Open311), collaborative maps, and appointment booking directly through AI.

## Description
Connect to the **Ayuntamiento de Zaragoza** (Zaragoza City Council) Open Data platform to interact with city services, public datasets, and administrative workflows through natural language.

### What you can do

- **Public Datasets** — Query information on monuments, restaurants, city equipment, and more using the `query_dataset` tool.
- **Citizen Services (Open311)** — Submit complaints or suggestions (`submit_open311_request`) and track their status directly from your agent.
- **Collaborative Maps** — List and inspect public or user-specific maps to visualize urban data.
- **Appointment Management** — Check availability for city services and book appointments (`book_appointment`) without navigating complex web forms.
- **Advanced Semantic Search** — Execute SPARQL queries for deep data analysis across the city's linked data infrastructure.

### How it works

1. Subscribe to this server
2. Provide your Zaragoza API Key and Client ID (optional for public data, required for citizen services)
3. Start querying city data or managing your administrative requests from any MCP-compatible client

### Who is this for?

- **Citizens** — report issues in the city or book appointments for municipal services easily.
- **Developers & Researchers** — access structured urban data and semantic datasets for analysis.
- **Tourists** — find monuments, restaurants, and points of interest with real-time city data.


## Available Tools
- **book_appointment**: Requires authentication.

Book an appointment (Cita Previa)
- **create_map**: Requires authentication.

Create a new collaborative map
- **delete_map**: Requires authentication.

Delete a collaborative map
- **execute_sparql_query**: zaragoza.es/sparql.

Execute a SPARQL query against Zaragoza Semantic Web endpoint
- **get_agenda_availability**: Get appointment availability for a specific day
- **get_agenda_detail**: Get details of a specific Cita Previa agenda
- **get_map_detail**: Get details of a collaborative map
- **get_my_appointments**: Get my booked appointments
- **get_open311_request**: Get details of a specific Open311 request
- **get_open311_service**: Get Open311 service definition
- **list_agendas**: List Cita Previa (Appointment) agendas
- **list_open311_requests**: List Open311 requests
- **list_open311_services**: List Open311 services (Quejas y Sugerencias)
- **list_public_maps**: List collaborative public maps
- **list_user_maps**: List collaborative maps for a specific user
- **query_dataset**: Query a generic Zaragoza dataset (e.g., restaurante, monumento)
- **submit_open311_request**: Requires authentication credentials.

Submit an Open311 request (Queja/Sugerencia)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ayuntamiento de Zaragoza** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for monuments in Zaragoza named 'Goya'."

**🤖 AI Agent:**
> I found several results for 'Goya' in the monuments dataset, including the 'Monumento a Goya' located in Plaza del Pilar. Would you like the full details or coordinates?

---

**👤 You:**
> "Report a cleaning issue at Calle Mayor 10 using Open311."

**🤖 AI Agent:**
> I've submitted the request for 'Cleaning and Waste' at Calle Mayor 10. Your service request ID is 12345. You can track its status using the `get_open311_request` tool.

---

**👤 You:**
> "Check availability for an appointment in the 'Padron' agenda for tomorrow."

**🤖 AI Agent:**
> Checking the 'Padron' agenda... There are 3 available slots tomorrow: 09:00, 10:30, and 11:15. Would you like me to book one of these for you?


## Installation & Usage

To install and use the **Ayuntamiento de Zaragoza** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayuntamiento-de-zaragoza](https://vinkius.com/mcp/ayuntamiento-de-zaragoza)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
