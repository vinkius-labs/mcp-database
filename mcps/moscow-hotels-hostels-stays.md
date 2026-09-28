# Moscow Hotels, Hostels & Stays MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-hotels-hostels-stays)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Keyless Moscow accommodation: hotels by star rating, hostels, short-stay apartments, guest houses and campsites, plus the Wikipedia hotel roll and a citywide profile.

## Description
Where to stay in Moscow, keyless — about 500 mapped hotels (a few dozen of them five-star), hostels, short-stay apartments and the outer-ring campsites.

### What you can do
- **find_hotels** — hotels (about 500) filtered by star rating and name, with phone, website and address
- **find_hostels** — hostels — the mapped subset of the budget market, with contacts and addresses
- **find_apartments** — short-stay apartments tagged in OSM — useful, but the tag is used inconsistently
- **find_budget_stays** — guest houses, motels, campsites, chalets and alpine huts — pick a kind or take the mix
- **hotels_wiki** — the Russian Wikipedia roll of Moscow hotels, with a short encyclopaedia entry for the first
- **accommodation_profile** — citywide counts of hotels, five-star hotels, hostels, apartments, guest houses, motels and campsites in one call

### Who is this for
Travellers comparing where to stay, and hosts advising visitors — which hotels are within walking distance of a venue, what five-star options exist.


## Available Tools (6)
- **accommodation_profile**: Use it to size the city for a stay question ("how many five-star hotels are mapped in Moscow?") without paging through lists. No filters — this is a profile, not a search.

Citywide Moscow accommodation profile
- **find_apartments**: Each row carries the name, phone, website, address and the coordinate. Filter by name fragment or narrow to a district with lat/lon/km. This tag is used inconsistently — many short-let flats are mapped as apartments with no tourism tag and will not appear here.

Find Moscow short-stay apartments
- **find_budget_stays**: Each row carries the name, phone, website, address and the coordinate. Filter by kind (e.g. "camp_site") or narrow to a district with lat/lon/km. The camping options sit mostly at the city edge, so a km filter around a suburban coordinate works best.

Find Moscow guest houses, motels and campsites
- **find_hostels**: Each row carries the name, phone, website, address and the coordinate. Filter by name fragment or narrow to a district with lat/lon/km. Hostel tagging in Moscow is thin compared with hotels — treat this as the mapped subset, not the complete market.

Find Moscow hostels
- **find_hotels**: Each row carries the name, star rating, phone, website, address and the centre coordinate. Filter by star rating (stars: "5", "4", "3"), by name fragment (e.g. "Метрополь", "Балчуг") or find the hotels around a venue with lat/lon/km. Not every mapped hotel carries a star tag, so the stars filter is a keep-only filter, not an exhaustive classification.

Find Moscow hotels
- **hotels_wiki**: Pass detail: "true" to fetch the summary of the first listed hotel.

Moscow hotel roll from Russian Wikipedia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Hotels, Hostels & Stays** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which five-star hotels are near the Bolshoi?"

**🤖 AI Agent:**
> find_hotels with stars: "5" and the Bolshoi coordinates plus km: "2" returns the mapped five-star options with phone and address.

---

**👤 You:**
> "Tell me about the Metropol hotel."

**🤖 AI Agent:**
> hotels_wiki with detail: "true" returns the Wikipedia entry for the first listed hotel; find_hotels with name: "Метрополь" locates it on the map.

---

**👤 You:**
> "How many hotels does Moscow have?"

**🤖 AI Agent:**
> accommodation_profile returns the citywide counts in one call — about 500 mapped hotels, including the five-star total.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: Can I book through this MCP?**
No. This is the mapped inventory — locations, names, phones, websites, star ratings. Booking happens on the hotel site or an aggregator.

**Q: Why is the star filter not exhaustive?**
Not every mapped hotel carries a star tag in OSM. The filter keeps only the ones that do, so a "5-star" search shows the mapped five-star hotels, not every five-star hotel in the city.

**Q: Can I find hotels near a venue?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-hotels-hostels-stays](https://vinkius.com/en/ai-agent-connect/moscow-hotels-hostels-stays)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Hotels, Hostels & Stays** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-hotels-hostels-stays` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Hotels, Hostels & Stays** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-hotels-hostels-stays": {
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
