# Ayuntamiento de Zaragoza MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ayuntamiento-de-zaragoza)
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


## ❓ FAQ

**Q: How can I find specific monuments or restaurants in Zaragoza?**
Use the `query_dataset` tool. You can specify the dataset (e.g., 'monumento' or 'restaurante') and apply filters like 'q' for names or 'point' and 'distance' for proximity searches.

**Q: Can I report a broken street light or a pothole using this server?**
Yes! Use the `submit_open311_request` tool. You'll need to provide the `service_code` (which you can find via `list_open311_services`) and a description of the issue.

**Q: How do I check if there are available slots for a city hall appointment?**
First, list available agendas with `list_agendas`, then use `get_agenda_availability` with the specific agenda ID to see open time slots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayuntamiento-de-zaragoza](https://vinkius.com/mcp/ayuntamiento-de-zaragoza)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ayuntamiento de Zaragoza** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ayuntamiento-de-zaragoza` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ayuntamiento de Zaragoza** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ayuntamiento-de-zaragoza": {
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
