# Geocodio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geocodio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Empower geocoding via Geocodio — perform batch geocoding and reverse geocoding for US/Canada, and retrieve Census and legislative data directly from any AI agent.

## Description
Connect your **Geocodio** account to any AI agent and take full control of your North American geocoding, address validation, and Census data workflows through natural conversation.

### What you can do

- **Geocoding Orchestration** — Identify bounded routing spaces inside the headless Geocodio US/CA maps and extract explicitly attached REST arrays targeting `/geocode` formatting string locations into valid North American coordinate blocks natively
- **Enriched Data Extraction** — Perform structural extraction of properties driving active Census domains, grabbing explicit demographics (ACS), timezones, or state legislative layouts flawlessy
- **Reverse Geocoding** — Retrieve explicit cloud logs tracing US/Canada coordinates to track exactly what address forms match GPS pins securely resolving street grids
- **Batch Processing Oversight** — Explains explicitly mapped arrays checking Geocodio POST requests processing high-volume arrays mapping up to 10,000 physical locations cheaply
- **Legislative & School Auditing** — Executes bulk iterations tracking explicitly registered Congressional Districts mapping `fields=cd` determining exactly who represents a GPS pin flawlessly
- **Census Block Mapping** — Commands explicit JSON targets tracking batch logic mapping multiple ACS limits pulling full neighborhood statistics efficiently
- **Supported Field Discovery** — Validates API logic querying exactly what fields Geocodio supports pulling hardcoded bounds informing your agent what data can be requested synchronously

### How it works

1. Subscribe to this server
2. Enter your Geocodio API Key (found in your Geocodio Dashboard)
3. Start geocoding and enriching your North American address data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — geocode thousands of addresses and append Census or legislative data without manual spreadsheet uploading
- **Real Estate & Logistics Teams** — perform reverse geocoding and analyze neighborhood demographics using natural language
- **Developers** — test and debug geocoding API parameters and verify address validation schemas through natural conversation
- **Campaign & Compliance Managers** — verify congressional districts and state legislative boundaries for large datasets in real-time


## Available Tools (10)
- **batch_reverse_pins**: Retrieve the exact structural matching verifying Delivery alternatives
- **format_coordinate_string**: Provision a highly-available JSON Payload parsing accessible strings
- **geocode_us_address**: Identify bounded routing spaces inside the Headless Geocodio US/CA maps
- **geocode_enriched_fields**: Perform structural extraction of properties driving active Census domains
- **list_schema_fields**: Irreversibly vaporize explicit validations extracting rich schema
- **reverse_geocode**: Retrieve explicit Cloud logging tracing explicit US/Canada coordinates
- **reverse_enriched_fields**: Enumerate explicitly attached structured rules exporting active Districts
- **batch_enriched_geocode**: Inspect deep internal arrays mitigating specific Timezone pipelines
- **batch_geocode_addresses**: Identify precise active arrays spanning native Location geometries
- **batch_enriched_reverse**: Dispatch an automated validation check routing explicit Census models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geocodio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode this address: '1109 N Highland St, Arlington, VA'"

**🤖 AI Agent:**
> Address geocoded! The coordinates for 1109 N Highland St are Lat: 38.88667, Lng: -77.0944. This location is now mapped into valid coordinate blocks for your analysis.

---

**👤 You:**
> "Reverse geocode '38.886, -77.094' and show me the Congressional District"

**🤖 AI Agent:**
> Reverse geocoding complete! The address is '1109 N Highland St, Arlington, VA'. This location belongs to Virginia's 8th Congressional District. Would you like the representative's name?

---

**👤 You:**
> "Get economic data for this address: 'White House, DC'"

**🤖 AI Agent:**
> Retrieving Census data... For the White House area, the ACS economics data shows a median household income of $120k+ and an unemployment rate of 3.2%. I can provide full neighborhood statistics for this block.


## ❓ FAQ

**Q: Can my agent geocode multiple addresses at once using Geocodio?**
Yes. Use the 'batch_geocode_addresses' tool and provide a JSON array of address strings. Geocodio handles up to 10,000 locations per request, allowing for high-throughput data enrichment natively.

**Q: How do I retrieve demographic data for an address via chat?**
Use the 'geocode_enriched_fields' tool. Provide the address and include 'acs-demographics' in the 'fields' parameter. The agent will analyze the active Census domains and return neighborhood statistics flawlessly.

**Q: Can I find the Congressional District for a set of GPS coordinates through the agent?**
Absolutely. Use the 'reverse_enriched_fields' tool. Provide the latitude and longitude and include 'cd' in the 'fields' parameter. Your agent will execute bulk iterations to determine exactly who represents that GPS pin natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geocodio](https://vinkius.com/mcp/geocodio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geocodio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geocodio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geocodio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geocodio": {
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
