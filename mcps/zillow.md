# Zillow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zillow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search US residential and rental properties — find homes by address, city or zipcode with pricing and property details.

## Description
Connect to **Zillow** and explore US real estate through natural conversation.

### What you can do

- **Property Search** — Search residential properties by address, city, state and zipcode
- **Property Details** — Get full property info including price, bedrooms, bathrooms, square footage and year built
- **Rental Search** — Search rental properties with rent prices, bedrooms, bathrooms and property details

### How it works

1. Subscribe to this server
2. Enter your Zillow Bridge API Key
3. Start exploring real estate data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Buyers** — search properties by location, compare prices and explore neighborhoods
- **Real Estate Agents** — find property details, pricing history and listing information
- **Renters** — search rental properties with pricing and amenity details


## Available Tools
- **get_property_by_id**: Returns full property details including address, price history, tax info, features, description and photos.

Get detailed info for a specific property by ID
- **get_rental_property**: Returns rental listings with rent price, bedrooms, bathrooms, square footage, property type and listing details.

Search for rental properties
- **search_property**: Returns property details including address, price, bedrooms, bathrooms, square footage, lot size, year built, property type and listing status.

Search for residential properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zillow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for properties in New York, NY."

**🤖 AI Agent:**
> Found 25 properties in New York, NY. Price range: $450K - $5.2M. Types: Condos, Townhouses, Single Family. Each with address, price, bedrooms, bathrooms and square footage.

---

**👤 You:**
> "Find rental properties in Los Angeles, CA."

**🤖 AI Agent:**
> Found 20 rental listings in Los Angeles, CA. Rent range: $1,800 - $8,500/month. Types: Apartments, Houses, Condos. Each with rent price, bedrooms, bathrooms and square footage.

---

**👤 You:**
> "Get details for property ID 12345."

**🤖 AI Agent:**
> Property 12345: 123 Oak Street, Los Angeles, CA 90001. Price: $1,250,000. 4 bed, 3 bath, 2,400 sqft. Built 2015. Single Family. Lot size: 5,200 sqft.


## ❓ FAQ

**Q: How do I get a Zillow API key?**
Apply for access through the [**Zillow Bridge API**](https://bridge.intercom.io/) program. You'll need to create an account and request API access.

**Q: Can I search properties by city?**
Yes! Use search_property with the city parameter to find all properties in a city. You can also filter by state and zipcode for more precise results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zillow](https://vinkius.com/mcp/zillow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zillow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zillow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zillow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zillow": {
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
