# Paris Sports: Public Facility Time Slots MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-sports-public-facility-time-slots)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless data on the ~18,800 time slots that Paris sports associations occupy in city-run facilities — discipline, weekday, hours, paid/free flag, age bounds and facility location.

## Description
The occupancy of Paris's public sports facilities by local associations and clubs — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_sport_slots / count_sport_slots** — the ~18,800 slot rows: the association name, discipline as stored (UPPERCASE — "TENNIS", "NATATION", "BASKET BALL", "JUDO"…), the weekday (lowercase French), start/end times, the facility (name, address, postal code), paid/free flag, gender, age bounds and the average annual price
- **free_sport_slots** — only the unpaid slots (about 7,800), same filters, to answer "what can I do in Paris for free on a Saturday"
- **sport_equipment_lookup** — all the slots held at one facility (e.g. "Gymnase Huyghens"), up to 100 rows per page
- **slots_by_age** — the slots whose stored age minimum/maximum equals a given value (the age columns are text: exact match only, no range queries)

### Who is this for
Families and solo adults looking for a free or nearby club activity, journalists on Paris's sports landscape, and anyone mapping which disciplines run in a given facility. Filters match stored values exactly — disciplines UPPERCASE, weekdays lowercase French — and page with limit (max 100) plus offset.


## Available Tools (5)
- **free_sport_slots**: Use it to answer "what free sports can I do in Paris on weekends".

List the free (unpaid) sports time slots
- **list_sport_slots**: Each row has the association/club name, the discipline as stored (UPPERCASE, e.g. "TENNIS", "NATATION", "BASKET BALL", "JUDO", "FOOTBALL A 11"), the weekday (jour_de_la_semaine, lowercase French, e.g. "mercredi"), the slot start/end times ("18:00:00"), the facility name (nom_de_l_equipement, e.g. "Gymnase Huyghens"), where inside the facility it happens (lieu_de_pratique_dans_l_equipement) and the facility address (adresse_de_l_equipement), its postal code (code_postal_de_l_equipement, "750xx"), whether the slot is paid (payant: "oui" or "non"), the gender (genre, "Mixte", "Homme" …), the age bounds (age_minimum / age_maximum, stored as text) and the average annual price in euros. Filters are exact stored values; page with limit/offset (100 rows max per call).

List sports-association time slots in Paris facilities
- **slots_by_age**: Combine with discipline or equipement to narrow it down. Use it to answer "what can an 8-year-old do" (age_min=8 or age_max=8).

Find sports slots for a given age
- **sport_equipment_lookup**: g. "Gymnase Huyghens" or "Tennis Jules Ladoumègue"), with the occupying association, discipline, weekday and hour windows, and the paid/free flag. Use list_sport_slots first to discover the exact stored facility name. Returns up to 100 rows; page through the facility's slots with offset if it runs long.

Find the time slots of one sports facility
- **count_sport_slots**: A fast total count — use it to compare slot volumes between disciplines or arrondissements.

Count sports time slots, optionally filtered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Sports: Public Facility Time Slots** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What free sports can I do on a Saturday in Paris?"

**🤖 AI Agent:**
> Call free_sport_slots with jour_de_la_semaine "samedi" and page through — each row has the discipline, facility, hours and the association that runs the slot.

---

**👤 You:**
> "Which facility runs gym sessions for 5-to-9-year-olds?"

**🤖 AI Agent:**
> Query slots_by_age with age_min "5" and discipline "GYMN ARTISTIQUE" (list_sport_slots shows the discipline labels — some have spaces, like "BASKET BALL"), then group the returned facilities.

---

**👤 You:**
> "What occupies the Gymnase Suchet, and when is it free of charge?"

**🤖 AI Agent:**
> sport_equipment_lookup with equipement "Gymnase Suchet" returns every slot at that facility; check the payant "non" rows among them (or filter the same facility through free_sport_slots) for the free ones.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: Why can I not filter slots between ages 8 and 12?**
The age_minimum / age_maximum columns are stored as text, and the ODS platform rejects range comparisons on text columns. slots_by_age matches the stored bound exactly (age_min 8 → slots starting at 8) — chain a few calls to cover a band.

**Q: Is this a live booking system?**
No. It is the city's occupancy reference: which association occupies which facility, on which weekday and hours, and whether the slot is paid. It is not a booking API.

**Q: How do I find all free tennis slots in the 16th?**
Run free_sport_slots with discipline "TENNIS" and code_postal "75016" — the facility postal code is a stored value you can filter on, and the free tool pins payant "non" automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-sports-public-facility-time-slots](https://vinkius.com/en/ai-agent-connect/paris-sports-public-facility-time-slots)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Sports: Public Facility Time Slots** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-sports-public-facility-time-slots` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Sports: Public Facility Time Slots** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-sports-public-facility-time-slots": {
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
