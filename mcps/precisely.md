# Precisely MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/precisely)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Equip your AI with precise location intelligence — geocode addresses, resolve property risks, calculate local taxes, and analyze demographics globally.

## Description
Fuse the **Precisely** geospatial intelligence network directly into your AI workflows, enabling your agents to accurately pinpoint addresses globally, extract demographics, and evaluate location-based risks with unparalleled precision.

### What you can do

- **Geocoding & Autocompletion** — Supply partial strings and tell the AI to resolve absolute Coordinates globally (`geocode_address`, `autocomplete_address`)
- **Risk Assessment** — Submit coordinates to instantly read FEMA flood zones or comparative crime metrics for that property (`enrich_flood_risk`, `enrich_crime_risk`)
- **Tax Boundaries** — Ask the AI to parse the exact Local Sales Tax jurisdiction applying strictly to that rooftop coordinate (`get_local_tax`)
- **Deep Enrichment** — Convert standard US Addresses into comprehensive property records including square footage and household socioeconomic segments

### How it works

1. Subscribe to this MCP server
2. Provide your Precisely API Key and API Secret
3. Start using conversational coordinates in Claude, Cursor, or your preferred agent

Stop managing external map APIs or relying on outdated geocoders. Simply tell the AI to 'verify the delivery status of 1600 Pennsylvania Ave' and let Precisely evaluate it natively.

### Who is this for?

- **Data Engineers** — standardize, clean, and verify raw address fragments spanning millions of global records without writing cURL scripts
- **Real Estate Analysts** — ask for property dimensions, flood scores, and socioeconomic stats in natural language to build instant reports
- **E-commerce Ops** — validate rooftop tax zones resolving complex US jurisdictions directly during development


## Available Tools
- **autocomplete_address**: Returns up to 10 candidate addresses ranked by relevance. Designed for keystroke-by-keystroke usage in address input forms.

Provide real-time address suggestions as users type using the Precisely Typeahead Autocomplete API, drawing from a comprehensive global address database to accelerate form completion and reduce entry errors
- **enrich_crime_risk**: Returns crime indices normalized to a national average of 100 — values above 100 indicate higher-than-average risk.

Assess the crime risk index for a specific location using the Precisely Risks API, returning normalized risk scores across categories like burglary, assault, vehicle theft, and overall crime relative to national averages
- **enrich_demographics**: Returns rich socio-economic profiles for the census block or postal zone containing the coordinates.

Retrieve detailed demographic segmentation data for a geographic coordinate using the Precisely Demographics API, including household income brackets, population density, education levels, age distribution, and consumer spending patterns
- **enrich_flood_risk**: Returns flood zone classification (A, AE, X, V), base flood elevation, and risk index. Primarily covers US territories with FEMA data.

Evaluate flood risk exposure for a specific location using the Precisely Environmental Risks API, returning FEMA flood zone designations, proximity to water bodies, elevation data, and flood risk scores
- **geocode_address**: precisely.com. The API returns a ranked list of candidates with latitude, longitude, precision code, and match confidence. Always pass the most complete address string available to maximize match quality. The response includes PrecisionCode indicating match depth (S8 = rooftop, S5 = street-level).

Forward-geocode a full or partial address string into geographic coordinates using the Precisely Geocoding API v1, which resolves against a world-class global address reference database covering 250+ countries and territories
- **get_local_tax**: Returns the combined tax rate and individual components (state, county, city, special district).

Determine the applicable sales tax rate and tax jurisdiction for a geographic location using the Precisely Local Tax API, resolving complex overlapping US tax jurisdictions down to the rooftop level
- **get_property_info**: Returns a rich property record sourced from county assessor databases. Coverage is US-only.

Retrieve comprehensive property attribute data for a US address using the Precisely Property API v2, including lot size, building square footage, year built, number of bedrooms/bathrooms, assessed value, and ownership information
- **reverse_geocode**: Note the parameter order: x = longitude, y = latitude. Returns the closest matching address with full components (street, city, state, postal code, country).

Convert geographic coordinates (latitude/longitude) back into a structured postal address using the Precisely Reverse Geocoding API, resolving the nearest rooftop-level address from the global reference database
- **get_timezone**: Returns the IANA timezone identifier (e.g. America/New_York), current UTC offset, and DST status.

Resolve the timezone and current UTC offset for any geographic coordinate using the Precisely Timezone API, accounting for daylight saving time transitions and political boundary changes
- **verify_address**: Returns a verified, standardized address with a verification status indicating if the address is deliverable, if components were corrected, or if the address is invalid.

Validate and standardize a postal address against authoritative reference datasets using the Precisely Address Verification API, returning USPS/Royal Mail/local postal authority standardized formatting and deliverability status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Precisely** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the exact sales tax for an e-commerce order delivered to '1 Market St, San Francisco, CA'?"

**🤖 AI Agent:**
> First I geocoded '1 Market Street, San Francisco, CA'. I retrieved coordinates `37.794, -122.395`. Evaluating `get_local_tax`, the combined sales tax rate there is exactly 8.625% (State: 6.0%, County: 0.25%, City: 1.25%, Special: 1.125%).

---

**👤 You:**
> "Check the crime risk around the latitude 40.7128 and longitude -74.0060 relative to the national average."

**🤖 AI Agent:**
> I queried `enrich_crime_risk` for `40.7128, -74.0060` (Lower Manhattan). The overall crime index is 231, meaning the risk is 2.3x higher than the national baseline score of 100. The highest driver is the Personal Property theft index.

---

**👤 You:**
> "Can you verify if '350 5th Ave New York 10118' is a real deliverable address? If yes, give me its timezone."

**🤖 AI Agent:**
> Using `verify_address`, I confirm it standardizes perfectly to '350 5TH AVE, NEW YORK, NY 10118-0110' (The Empire State Building), fully deliverable. Extracting `get_timezone` with its coordinates, it operates under `America/New_York` (UTC-05:00).


## ❓ FAQ

**Q: Can the AI find out if a specific property is inside a flood zone?**
Yes. First the AI uses `geocode_address` to find the exact Latitude/Longitude of the building's rooftop. Then it feeds those coordinates into `enrich_flood_risk` to extract the strict FEMA designation naturally.

**Q: How accurately does verify_address standardize locations?**
Very accurately. It connects to native postal services (like USPS and Royal Mail) to autocorrect misspellings, adjust zip codes, and flag impossible addresses before they reach your logistics layer.

**Q: Do I need two separate keys to use this?**
Yes. Precisely Developer APIs use robust OAuth workflows. You must supply both the individual API Key (Consumer Key) and the API Secret. The MCP server handles token exchanging for you internally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/precisely](https://vinkius.com/mcp/precisely)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Precisely** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `precisely` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Precisely** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "precisely": {
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
