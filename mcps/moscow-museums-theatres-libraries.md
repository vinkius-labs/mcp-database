# Moscow Museums, Theatres & Libraries MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-museums-theatres-libraries)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culture](../categories/culture.md)

Keyless Moscow culture: museums (by collection type), theatres, libraries, curated Wikipedia listings and a short encyclopaedia entry for each institution.

## Description
Moscow’s cultural map and its encyclopaedia, keyless — about 500 museums, 320 theatres and 660 libraries mapped, plus the curated Wikipedia categories.

### What you can do
- **find_museums** — museums (about 500) filtered by collection type — art, history, science, local, biographical, military and more — plus name, open now and proximity
- **find_theatres** — theatres and concert halls (about 320) filtered by stage type (opera, ballet, drama) and name
- **find_libraries** — libraries (about 660), from the Russian State Library (Ленинка) to district branches
- **culture_category_listing** — the curated Russian Wikipedia listings of Moscow museums, theatres and libraries
- **cultural_institution** — a short Wikipedia entry for one institution — title, one-line description and introductory paragraph in Russian

### Who is this for
Visitors and residents planning culture in Moscow: what’s near the hotel, which museums are open, or a short authoritative text about a venue.


## Available Tools (5)
- **cultural_institution**: g. "Третьяковская галерея", "Большой театр", "Музей космонавтики", "Парк Горького"). Use culture_category_listing to discover titles first. The text is Wikipedia's intro — for opening hours and tickets use find_museums or the venue's own site.

Summarise a Moscow cultural institution (Wikipedia)
- **culture_category_listing**: Returns the page titles; pass a title to cultural_institution for the short description and extract. Wikipedia is the curated view; find_museums / find_theatres / find_libraries give the map view with coordinates.

List cultural institutions of Moscow (Wikipedia)
- **find_libraries**: Filter by name fragment or by proximity to a point. Each row carries the name, operator, phone, opening hours and the centre coordinate.

Find libraries in Moscow
- **find_museums**: Filter by collection type — museum: "art", "history", "science", "natural_history", "local", "biographical", "maritime", "military", "war", "toy", "music", "photo" or "archaeology" — by name fragment, or by proximity to a point. Each row carries the name, phone, website, opening hours and the centre coordinate. Wikipedia has a longer curated list (120+ entries) — use culture_category_listing for it.

Find museums in Moscow
- **find_theatres**: Filter by stage type — theatre: "theatre", "opera", "ballet", "operetta", "circus", "cabaret" or "variety" — by name fragment, or by proximity to a point.

Find theatres in Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Museums, Theatres & Libraries** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which art museums are open near the centre?"

**🤖 AI Agent:**
> find_museums with type: "art", open_now: "true" and the centre coordinates lists them by proximity with hours and phone.

---

**👤 You:**
> "Tell me about the Tretyakov Gallery."

**🤖 AI Agent:**
> cultural_institution with the Russian title returns the Wikipedia summary: title, one-line description and introductory paragraph.

---

**👤 You:**
> "How many theatres does Moscow have?"

**🤖 AI Agent:**
> find_theatres returns the citywide count in one call (the map records about 320); culture_category_listing adds Wikipedia’s curated 32-entry list.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Why two views — map and Wikipedia?**
The listings come from Russian Wikipedia’s curated categories (120+ museums, 32 theatres, 37 libraries). The find_* tools give the map view with coordinates; the listing tools give the curated encyclopaedia view.

**Q: Why are the counts bigger than the rows I get?**
Yes. OSM maps most large venues as areas (museum buildings, theatre blocks), and every list tool uses the nwr selector, so nodes, ways and relations all count.

**Q: Can I find museums near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-museums-theatres-libraries](https://vinkius.com/en/ai-agent-connect/moscow-museums-theatres-libraries)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Museums, Theatres & Libraries** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-museums-theatres-libraries` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Museums, Theatres & Libraries** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-museums-theatres-libraries": {
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
