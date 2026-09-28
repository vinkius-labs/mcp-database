# Moscow History, Heritage & High-Rises MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-history-heritage-high-rises)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Keyless Moscow heritage: historic buildings and manors, monuments and plaques, archaeological sites and the high-rise inventory, plus the Wikipedia architecture roll.

## Description
Nine centuries of building, keyless — about 1,100 tagged historic buildings and manors, over 2,000 monuments and memorials, and the Stalinist high-rise inventory.

### What you can do
- **find_historic_buildings** — historic buildings, manors, castles and palaces (about 1,100) with architect, construction date and heritage status
- **find_memorials** — monuments and memorials (over 2,000), including every Great Patriotic War memorial, by name or kind
- **find_plaques** — commemorative plaques — the "on this building lived..." signs that cover central Moscow
- **find_archaeology** — archaeological sites, ruins and historic boundary stones — a small, mostly central set
- **find_high_rises** — the tall-building inventory from 12 floors up — the Seven Sisters, the Moscow City towers, the late-Soviet giants
- **architecture_wiki** — the Russian Wikipedia roll of Moscow architectural monuments, with a short encyclopaedia entry for the first

### Who is this for
Walkers who look up, architecture students, tour planners and anyone curious about who lived behind a facade in central Moscow.


## Available Tools (6)
- **architecture_wiki**: Pass detail: "true" to fetch the summary of the first listed building.

Moscow architecture roll from Russian Wikipedia
- **find_archaeology**: Each row carries the name, the site type and the coordinate. Sparse by nature — Moscow has a handful of mapped sites, mostly the excavated White City foundations and old estate ruins. Filter by name fragment or narrow to a district with lat/lon/km.

Find Moscow archaeological sites and ruins
- **find_high_rises**: Covers the Stalinist high-rises, the Moscow City towers and the late-Soviet housing giants — the Seven Sisters all carry 20+ floors. Each row carries the name, architect, construction date, the mapped floor count and the coordinate. Pass min_floors to change the tier (default 20). Note the tier is a regex over the levels tag, so buildings with an unmapped floor count are invisible to this tool.

Find Moscow tall buildings by floor count
- **find_historic_buildings**: Each row carries the name, architect, construction date, heritage status and coordinate. Filter by name fragment (e.g. "усадьба", "Пашков") or narrow to a district with lat/lon/km. For the full architecture roll use architecture_wiki.

Find Moscow historic buildings, manors and palaces
- **find_memorials**: Each row carries the name, the memorial subject where mapped and the coordinate. Filter by name fragment (e.g. "Победы", "Гагарину") or narrow to a district with lat/lon/km. Commemorative plaques are a separate tool.

Find Moscow monuments and memorials
- **find_plaques**: " signs that cover central Moscow). Each row carries the inscription where mapped and the coordinate. Filter by name fragment (e.g. "Пушкин", "Чехов") or narrow to a street with lat/lon/km. Coverage is thickest inside the Garden Ring; the outer districts are sparsely plaqued.

Find Moscow commemorative plaques


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow History, Heritage & High-Rises** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the Stalinist high-rises."

**🤖 AI Agent:**
> find_high_rises with min_floors: "20" returns the tall-building inventory; the Seven Sisters all carry 20 floors or more.

---

**👤 You:**
> "Whose memorial plaques are on this street?"

**🤖 AI Agent:**
> find_plaques with the street coordinates and a small km radius returns the mapped plaques with their inscriptions.

---

**👤 You:**
> "What historic estates are there in Moscow?"

**🤖 AI Agent:**
> find_historic_buildings with kind: "manor" lists the mapped estates — Kuskovo, Ostankino, Tsaritsyno — with architect and date.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: Is the heritage list official?**
The map layer is the volunteer view; the protected list is Russian Wikipedia’s category of architectural monuments. For an official register, Moscow’s own portal refuses connections from outside Russia.

**Q: Why do some high-rises not appear?**
The floor filter is a regex over the building:levels tag. Buildings whose level count is unmapped in OSM are invisible to this tool, whatever their real height.

**Q: Can I find monuments near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-history-heritage-high-rises](https://vinkius.com/en/ai-agent-connect/moscow-history-heritage-high-rises)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow History, Heritage & High-Rises** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-history-heritage-high-rises` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow History, Heritage & High-Rises** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-history-heritage-high-rises": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
