# Idealista (Real Estate) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/idealista-real-estate)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/idealista-real-estate-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/idealista-real-estate-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Search real estate via Idealista — find homes, commercial premises, and new developments in Spain, Italy, and Portugal.

## Description
Connect your **Idealista** developer account to any AI agent and take full control of your real estate searches and market analysis through natural conversation.

### What you can do

- **Geo-Spatial Search** — Find properties using precise GPS coordinates and a search radius, filtering by price and size directly from your agent
- **Residential Sales** — Search for homes and apartments for sale in specific zones (location_id) with filters for minimum rooms and maximum price
- **Rental Market** — Access updated rental listings to find houses or apartments available for lease in your target areas
- **Commercial Premises** — Discover commercial real estate opportunities, including offices and warehouses, for sale or rent
- **New Developments** — Explore residential projects under construction or recently finished to stay ahead of the market
- **Multi-Country Support** — Seamlessly navigate real estate markets across Spain (es), Italy (it), and Portugal (pt)

### How it works

1. Subscribe to this server
2. Enter your Idealista API Key and Secret
3. Start searching for properties from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Investors** — analyze market opportunities and find undervalued assets through natural conversation
- **Relocation Agents** — search for rentals and homes for clients across multiple countries without manual searching
- **Real Estate Analysts** — monitor new developments and commercial trends in specific European regions efficiently


## Available Tools
- **buscar_inmuebles**: Opcionalmente puedes filtrar por precio y tamaño.

Buscar inmuebles por coordenadas GPS y radio
- **pisos_venta**: Utilízalo para encontrar propiedades en venta disponibles para compra.

Buscar pisos en venta por zona
- **pisos_alquiler**: Muestra resultados actualizados de mercado.

Buscar pisos en alquiler
- **obra_nueva**: Ayuda al usuario a descubrir proyectos residenciales en construcción o recién terminados.

Buscar promociones de obra nueva
- **locales_comerciales**: Por defecto busca en alquiler si no se especifica.

Buscar locales comerciales


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Idealista (Real Estate)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for apartments for rent in Madrid with a maximum price of 1500 euros"

**🤖 AI Agent:**
> I've found several apartments for rent in Madrid matching your budget. Highlights include a 2-bedroom flat in Chamberí (€1,450), a modern studio in Malasaña (€1,200), and a bright apartment near Retiro (€1,500). Would you like the links to any of these?

---

**👤 You:**
> "Find homes for sale near these coordinates: 40.4167,-3.7033 within 1km"

**🤖 AI Agent:**
> Searching within 1000m of Central Madrid… I've identified 12 properties for sale. Prices range from €350,000 for a renovatable flat to €1.2M for a luxury penthouse. Would you like me to filter these by minimum size?

---

**👤 You:**
> "What are the new developments available in Lisbon?"

**🤖 AI Agent:**
> I've retrieved the latest new developments in Lisbon. Current projects include 'Tejo Riverside Residences', 'Chiado Legacy', and 'Belem Garden'. I can provide details on construction status and starting prices for any of these.


## Installation & Usage

To install and use the **Idealista (Real Estate)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/idealista-real-estate](https://vinkius.com/mcp/idealista-real-estate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
