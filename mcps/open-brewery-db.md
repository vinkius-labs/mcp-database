# Open Brewery DB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-brewery-db)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Discover breweries across the United States — search by name, city, state, or type with addresses, phone numbers, and websites for every location.

## Description
The **Open Brewery DB MCP Server** gives your AI agent access to a comprehensive, open-source database of breweries across the United States.

### Core Capabilities

- **Search by Name** — Find any brewery by name or keyword.
- **Filter by City** — Discover all breweries in San Diego, Portland, Denver, Austin, or any city.
- **Filter by State** — Browse breweries across California, Colorado, Oregon, Texas, New York, and all 50 states.
- **Filter by Type** — Explore micro-breweries, nano-breweries, regional breweries, brewpubs, contract brewers, and proprietor operations.
- **Contact Info** — Every brewery includes address, phone number, website, and GPS coordinates.

Zero authentication required. Free and open-source. Essential for travel, lifestyle, and hospitality AI agents.


## Available Tools
- **find_breweries_by_city**: Great for travel planning and local craft beer exploration.

Find all breweries in a specific city
- **find_breweries_by_state**: Use full state names (e.g. California, Colorado, Oregon, Texas, New York).

Find breweries in a specific state
- **find_breweries_by_type**: Find breweries by type (micro, nano, brewpub, regional, etc.)
- **search_breweries**: Covers micro-breweries, nano-breweries, regional breweries, brewpubs, and more across the United States.

Search for breweries by name or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Brewery DB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me craft breweries in Portland."

**🤖 AI Agent:**
> Portland is a craft beer paradise! I found 50+ breweries including: Deschutes Brewery (regional), Hair of the Dog Brewing (micro), Widmer Brothers (regional), and Cascade Brewing (micro). Each listing includes full address, phone, and website for planning your brewery tour.

---

**👤 You:**
> "List some nanobreweries in Colorado."

**🤖 AI Agent:**
> I found several nanobreweries in Colorado! Some options include: The Old Mine Cidery & Brewpub in Erie, Paradox Beer Company in Divide, and Nano 108 Brewing Company in Colorado Springs.

---

**👤 You:**
> "I need the address and website for Russian River Brewing in California."

**🤖 AI Agent:**
> Russian River Brewing Company is located at 725 4th St, Santa Rosa, CA 95404. You can visit their website at http://www.russianriverbrewing.com. They are categorized as a regional brewery.


## ❓ FAQ

**Q: What brewery types are available?**
Six types: micro (small-scale production), nano (ultra-small, often home-based), regional (large-scale distribution), brewpub (restaurant+brewery combo), contract (brewed at another location), and proprietor (owner-operated with minimal production).

**Q: Can I search for breweries by location coordinates?**
Yes, many entries in the Open Brewery DB include precise latitude and longitude coordinates, making it possible to query for breweries near a specific geographical point.

**Q: Are international breweries included?**
While the primary focus of Open Brewery DB has historically been the United States, it is actively expanding to include breweries from the UK, Ireland, South Korea, and other international locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-brewery-db](https://vinkius.com/mcp/open-brewery-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Brewery DB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-brewery-db` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Brewery DB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-brewery-db": {
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
