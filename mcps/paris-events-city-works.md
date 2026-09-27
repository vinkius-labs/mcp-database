# Paris Events & City Works MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-events-city-works)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [events](../categories/events.md)

Keyless Paris events data: the official "Que faire à Paris" program, the ~80 open-air markets, scheduled road closures and registered building works — filter by category, arrondissement and day.

## Description
The City of Paris's official event program, its open-air markets, and the city works calendar — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_events / count_events** — the "Que faire à Paris" program entries: event name, description, venue, start/end, category and access info; filter by price type, PMR accessibility, group format or access type, and count without fetching rows
- **event_program_summary** — the program's composition by category, venue and week, so you can discover the exact stored values to filter on
- **list_open_air_markets** — the ~80 street markets (the whole dataset fits in one call): what is sold, which arrondissement, the weekday it is held and weekly hours
- **list_road_closures** — scheduled road-closure periods per street, with the closure type and progress state
- **list_works / count_works** — the registered building works, filterable by arrondissement, work category and detailed location

### Who is this for
Trip planners answering "what is on in Paris" and "where can I buy fresh produce on a Wednesday", and anyone routing around a closed street or a declared work site. Every text filter matches a stored value exactly — use event_program_summary and the market weekday names (lundi..dimanche) to discover them. Page with limit (max 100) and offset.


## Available Tools (7)
- **count_events**: A fast total count — use it to gauge how many rows a filtered page of list_events covers before paging with offset.

Count "Que faire à Paris" entries, optionally filtered
- **count_works**: A fast total count — use it to gauge how much paging list_works will need.

Count registered building works, optionally filtered
- **event_program_summary**: Use it to discover the exact filter values for list_events (the counts show which groups actually carry content, e.g. "Bibliothèques" and "Agenda" dominate).

Summarize the "Que faire à Paris" program composition
- **list_events**: Each entry has the event title, the paris.fr event page URL, start/end dates, the price, accessibility flags and the venue. Recurring program entries leave date_start null and carry the schedule as text in date_description or occurrences. Use it to answer "what is on in Paris", with exact stored-value filters: price_type is "gratuit", "payant" or "gratuit sous condition"; group is "Bibliothèques", "Agenda", "Activités DJS", "Parcs et jardins", "Conservatoires", "Associations", "Fabrique de la solidarité", "Nuit Blanche", "Centres d'animations" or "Musées" (accents matter); access_type is "obligatoire", "conseillée" or "non"; pmr / blind / deaf are "1" (yes) or "0". The response includes the dataset total, so page further with offset (rows are capped at 100 per call).

List entries from the official "Que faire à Paris" program
- **list_open_air_markets**: Each market has the short/long name, what is sold (produit), the arrondissement it sits in, the location description, the days it is held (the jours_tenue text plus one 0/1 flag per weekday), the managing operator and the weekly hours. Use it to answer "where can I buy … in Paris" or "what markets are open on …". Filters are exact stored values: day is one of lundi, mardi, mercredi, jeudi, vendredi, samedi, dimanche; ardt is the arrondissement number as a string, "1".."20"; produit is "Alimentaire", "Alimentaire bio", "Fleurs", "Puces", "Timbres" or "Création artistique"; secteur is "A" or "B".

List Paris open-air markets
- **list_road_closures**: Each row has the closure type, the location name, the start/end instants (ISO), a human-readable period text, the affected direction (about half the rows have none) and the status. Filters are exact stored values: type_fv is "Bretelle", "Boulevard périphérique", "Tunnel" or "Voie sur berges"; etat_avancement is "Planifié", "En cours" or "Terminé"; sens_fv is "Périphérique intérieur", "Périphérique extérieur", "De Paris vers province" or "De province vers Paris". Page with limit/offset (100 rows max per call).

List scheduled Paris road-closure periods
- **list_works**: Each site has the permit number, the arrondissement (5-digit postal code, "75001".."75020"), the start and end dates (YYYY-MM-DD), the category, a short work description, the main client and the footprint locations (an array of "EMPRISE_CHAUSSEE", "EMPRISE_TROTTOIR" or "EMPRISE_PISTE_CYCLABLE"). Use it to answer "what works are happening around street X / arrondissement N". Filters are exact stored values: chantier_categorie is "Tiers (travaux sur bâtiment)", "Opérateurs de réseau (gaz-électricité-RATP-etc)" or "Ville de Paris (Tvx sur espace ou édifice public)"; cp_arrondissement is the 5-digit postal code; localisation_detail is one footprint value from the array above. Page with limit/offset (100 rows max per call).

List registered building works in Paris


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Events & City Works** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is on in Paris this week that is free?"

**🤖 AI Agent:**
> list_events with price_type: "Gratuit" returns the free "Que faire à Paris" entries, soonest first within the data — page with limit/offset; event_program_summary shows how many entries exist per category if you want to narrow the theme.

---

**👤 You:**
> "Where can I buy fresh produce in the 10th arrondissement on a Tuesday?"

**🤖 AI Agent:**
> list_open_air_markets with day: "mardi", ardt: "10" and produit: "Alimentaire" returns the food markets held on Tuesdays in that arrondissement, with their street, hours and operator.

---

**👤 You:**
> "Which building works are registered in the 8th arrondissement?"

**🤖 AI Agent:**
> list_works with cp_arrondissement: "8" returns the works registered in that arrondissement, with the work category and the detailed location (street or site); add chantier_categorie to narrow the type of work.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: What is the "Que faire à Paris" program?**
The City of Paris's official program of events, exhibitions and activities. list_events returns its entries (name, venue, start/end, category, access info) and event_program_summary breaks the program down by category, venue and week so you can find the exact filter values.

**Q: How do I find which markets are open on a given weekday?**
list_open_air_markets takes day as one of lundi, mardi, mercredi, jeudi, vendredi, samedi, dimanche, plus produit (e.g. "Alimentaire"), ardt (arrondissement "1".."20") and secteur ("A"/"B"). The whole market dataset (~80 rows) returns in one call.

**Q: How do I route around a closed street or a declared work?**
list_road_closures returns the scheduled closure periods per street with the closure type and progress state; list_works (or count_works) lists the registered building works, both filterable by arrondissement (cp_arrondissement "1".."20").


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-events-city-works](https://vinkius.com/en/ai-agent-connect/paris-events-city-works)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Events & City Works** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-events-city-works` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Events & City Works** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-events-city-works": {
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
