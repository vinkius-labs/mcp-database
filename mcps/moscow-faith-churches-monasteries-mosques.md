# Moscow Faith: Churches, Monasteries & Mosques MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-faith-churches-monasteries-mosques)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culture](../categories/culture.md)

Keyless Moscow faith: Orthodox and Christian churches by denomination, monasteries, mosques, synagogues and historic cemeteries, plus the Wikipedia monastery roll.

## Description
The religious map of the city, keyless — about a thousand Christian places of worship, forty monasteries, the mosques and synagogues, and the historic cemeteries.

### What you can do
- **find_churches** — Christian places of worship (about 1,000) filtered by denomination — russian_orthodox, roman_catholic, baptist, old_believers — and name
- **find_monasteries** — monasteries (about 40) — Novodevichy, Donskoy, Danilov, Andronikov — matched by tag and by name
- **find_mosques** — mosques and Muslim prayer rooms — the Cathedral Mosque, the Memorial Mosque and neighbourhood rooms
- **find_synagogues** — synagogues — the Choral Synagogue, the Memorial Synagogue on Poklonnaya Hill, the Zhukka centre
- **find_cemeteries** — historic cemeteries — Novodevichy, Vagankovo, Donskoy, Vvedenskoye — by name and religion
- **monasteries_wiki** — the Russian Wikipedia roll of Moscow monasteries, with a short encyclopaedia entry for the first
- **faith_profile** — citywide counts of churches, monasteries, mosques, synagogues, all worship places and cemeteries in one call

### Who is this for
Visitors exploring Orthodox heritage, residents looking for the nearest working church or mosque, and genealogists hunting a historic cemetery.


## Available Tools (7)
- **faith_profile**: Use it to size the city for a question ("how many mosques are mapped in Moscow?") without paging through lists. No filters — this is a profile, not a search.

Citywide Moscow faith profile
- **find_cemeteries**: Each row carries the name, religion where mapped and the coordinate as an area centre. Filter by name fragment (e.g. "Новодевичье", "Ваганьково") or narrow to a district with lat/lon/km. Several historic cemeteries are also parks — cross-reference with the environment MCP for the green-space view.

Find Moscow cemeteries and graveyards
- **find_churches**: Each row carries the name, denomination, opening hours, heritage status and the coordinate. Filter by denomination (e.g. "russian_orthodox", "roman_catholic", "baptist", "old_believers") or by name fragment (e.g. "Николая", "Воскресения"). For monasteries use find_monasteries.

Find Moscow Orthodox and Christian churches
- **find_monasteries**: Moscow has about forty active and former monasteries (Novodevichy, Donskoy, Danilov, Andronikov, Rogozhskoe). Each row carries the name, religion, denomination, heritage status and the coordinate. For the encyclopaedic roll use monasteries_wiki.

Find Moscow monasteries
- **find_mosques**: Each row carries the name, denomination, opening hours and the coordinate. Filter by name fragment or narrow to a district with lat/lon/km.

Find Moscow mosques
- **find_synagogues**: Each row carries the name, opening hours, website and the coordinate. Filter by name fragment or narrow to a district with lat/lon/km.

Find Moscow synagogues
- **monasteries_wiki**: Pass detail: "true" to fetch the summary of the first listed monastery.

Moscow monastery roll from Russian Wikipedia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Faith: Churches, Monasteries & Mosques** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which Orthodox churches are near the centre?"

**🤖 AI Agent:**
> find_churches with denomination: "russian_orthodox" and the centre coordinates lists them with hours and heritage status.

---

**👤 You:**
> "Tell me about Novodevichy Convent."

**🤖 AI Agent:**
> monasteries_wiki with detail: "true" returns the Wikipedia entry for the first listed monastery; find_monasteries locates it on the map.

---

**👤 You:**
> "Where is the nearest mosque?"

**🤖 AI Agent:**
> find_mosques with your coordinates and km: "10" returns the mapped mosques with hours; Moscow’s best-known are the Cathedral and the Memorial mosques.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: Are all Moscow churches Orthodox?**
The great majority are Russian Orthodox, but the city also maps Roman Catholic, Baptist, Old Believer, Lutheran and other Christian congregations. Filter by denomination to separate them.

**Q: Why do monasteries match by name as well as tag?**
Some monasteries are tagged amenity=monastery, others only as a place of worship whose name contains "монастырь". The tool unions both so neither set is lost.

**Q: Can I find churches near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-faith-churches-monasteries-mosques](https://vinkius.com/en/ai-agent-connect/moscow-faith-churches-monasteries-mosques)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Faith: Churches, Monasteries & Mosques** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-faith-churches-monasteries-mosques` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Faith: Churches, Monasteries & Mosques** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-faith-churches-monasteries-mosques": {
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
