# Georef Argentina MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/georef-argentina)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access official Argentine geographic data—normalize addresses, list administrative divisions, and perform reverse geocoding directly from your AI.

## Description
Connect your AI agent to the official **Georef Argentina** service to access precise geographic and administrative information. This server allows you to interact with the national database of provinces, departments, municipalities, and streets.

### What you can do

- **Administrative Hierarchy** — List and filter provinces, departments, and municipalities by name or ID using `get_provincias`, `get_departamentos`, and `get_municipios`.
- **Address Normalization** — Convert messy address strings into structured data with precise components using `normalize_direccion`.
- **Street Database** — Search for specific streets (vías) within any locality or department using `get_vias`.
- **Reverse Geocoding** — Provide latitude and longitude to identify the exact administrative location with `reverse_geocoding`.
- **Data Enrichment** — Fetch centroids and metadata for geographic entities to power maps and analytics.

### How it works

1. Subscribe to this server
2. Enter your Georef API Key (if required for high-volume access)
3. Start querying Argentine geography from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Delivery** — Normalize customer addresses to ensure accurate shipping and routing.
- **Data Analysts** — Clean and categorize datasets containing Argentine location information.
- **Developers** — Integrate official government geographic data without manual scraping or complex API setups.


## Available Tools
- **get_departamentos**: Get a list of departments in Argentina
- **normalize_direccion**: g., "Av. Mayo 100").

Normalize a full address string into its components
- **get_localidades**: Get a list of localities in Argentina
- **get_municipios**: Get a list of municipalities in Argentina
- **get_provincias**: Can filter by ID or name.

Get a list of provinces in Argentina
- **reverse_geocoding**: ) for lat/lon.

Get geographic location for a given set of coordinates
- **get_vias**: Get a list of streets (vías) in Argentina


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Georef Argentina** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all provinces in Argentina."

**🤖 AI Agent:**
> I've retrieved the list of provinces. Argentina has 24 main jurisdictions, including Buenos Aires, Córdoba, Santa Fe, and Mendoza. Would you like to see the IDs or centroids for any of them?

---

**👤 You:**
> "Normalize the address 'Av. 9 de Julio 1234, CABA'."

**🤖 AI Agent:**
> The address has been normalized. It corresponds to 'AVENIDA 9 DE JULIO 1234', located in the Autonomous City of Buenos Aires (CABA). The coordinates are Lat: -34.612, Lon: -58.381.

---

**👤 You:**
> "What is the location for coordinates -34.6037, -58.3816?"

**🤖 AI Agent:**
> Those coordinates correspond to the Obelisco area in the Autonomous City of Buenos Aires (CABA), specifically within the San Nicolás neighborhood.


## ❓ FAQ

**Q: Can I find the coordinates of a specific address string?**
Yes! Use the `normalize_direccion` tool. It will parse the address and return the structured components along with geographic coordinates.

**Q: How do I list all departments within a specific province?**
Use the `get_departamentos` tool and provide the province name or ID in the `provincia` parameter to filter the results.

**Q: Can I get the administrative location of a specific latitude and longitude?**
Yes, the `reverse_geocoding` tool takes `lat` and `lon` parameters and returns the corresponding province, department, and municipality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/georef-argentina](https://vinkius.com/mcp/georef-argentina)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Georef Argentina** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `georef-argentina` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Georef Argentina** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "georef-argentina": {
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
