# Moscow Public Services: Post, Banks, Notaries MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-public-services-post-banks-notaries)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [civic-tech](../categories/civic-tech.md)

Keyless Moscow public services: post offices, banks and on-site ATMs, cash machines, government offices by level, clinics and dentists, notaries, plus city institutions.

## Description
Moscow’s everyday services on a map, keyless — about 1,780 post offices, 3,000 ATMs, 930 tagged government offices, 400 notaries and 8,000 clinics and doctors.

### What you can do
- **find_post_offices** — post offices (about 1,780), mostly Russian Post branches, filterable by operator, name and open now
- **find_banks** — bank branches (about 410) filterable by name, on-site ATM and open now
- **find_atms** — cash machines (about 3,000) by operator — the practical tool, with a proximity search
- **find_government_offices** — government offices (about 930) by level — city, regional, national, prosecutor, tax, migration, register, courthouse
- **find_clinics** — clinics and doctors (about 8,000) filtered by mapped specialty — dentistry, paediatrics, gynaecology and more
- **find_notaries** — notary offices (about 400)
- **city_institution** — a short Wikipedia entry for a city institution — the mayor’s office, the city government, the city duma or the city court

### Who is this for
Residents handling bureaucracy: a post office, an ATM, a migration or tax office, a notary, or a clinic with the right specialty.


## Available Tools (7)
- **city_institution**: Returns the title, the one-line description and the introductory paragraph, in Russian. For the address of a service use the find_* tools — this is the encyclopaedia view.

Summarise a Moscow city institution (Wikipedia)
- **find_atms**: Each row carries the operator/brand and the coordinate, plus the cash-out and deposit flags when the map records them. ATMs are points, so a proximity search (lat + km, default 2 km) is the practical way to use this tool.

Find cash machines (ATMs) in Moscow
- **find_banks**: Each row carries the name, brand, phone, opening hours and the centre coordinate. Pass atm: "yes" to keep only branches with a mapped cash machine on site, or open_now for branches open at the moment of the call. For cash machines alone use find_atms.

Find bank branches in Moscow
- **find_clinics**: Each row carries the name, healthcare tag, phone, opening hours and the centre coordinate. Filter by specialty fragment (healthcare:specialty, e.g. "dentistry", "paediatrics", "gynaecology" — values are as mapped) or by open_now. For hospitals and emergency care use the safety MCP.

Find clinics and doctors in Moscow
- **find_government_offices**: Filter by level — government: "city" (Moscow city government), "regional", "national" (federal offices in the capital), "prosecutor", "tax", "migration", "register_office" or "courthouse" — or by name fragment. Each row carries the name, the government level, phone and the centre coordinate.

Find government offices in Moscow
- **find_notaries**: Each row carries the name, operator, phone, opening hours and the centre coordinate. A proximity search (lat + km) is the practical way to use this tool — pass the district centre or an address coordinate.

Find notary offices in Moscow
- **find_post_offices**: Each row carries the name, operator, phone, opening hours and the centre coordinate. Filter by operator fragment (e.g. "Почта России") or by open_now, and narrow to a radius with lat/km. Post offices are mostly mapped as points, so the count is close to complete.

Find post offices in Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Public Services: Post, Banks, Notaries** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is the nearest ATM?"

**🤖 AI Agent:**
> find_atms with your lat/lon (km defaults to 2) lists the mapped cash machines by distance, with operator and cash-out flags.

---

**👤 You:**
> "Which post offices are open now?"

**🤖 AI Agent:**
> find_post_offices with open_now: "true" keeps only the offices whose mapped hours cover the moment of the call; add an operator fragment for Russian Post.

---

**👤 You:**
> "Explain the Moscow city government to me."

**🤖 AI Agent:**
> city_institution with institution: "government" returns the Wikipedia summary in Russian — title, description and introductory paragraph.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: How do I find a migration or tax office?**
find_government_offices with level: "migration" or "tax" returns the offices tagged with that government level, with name, phone and coordinate.

**Q: How do I find a dentist nearby?**
find_clinics with specialty: "dentistry" and your lat/lon lists clinics and doctors tagged with that specialty, sorted by proximity.

**Q: Can I find services near me?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-public-services-post-banks-notaries](https://vinkius.com/en/ai-agent-connect/moscow-public-services-post-banks-notaries)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Public Services: Post, Banks, Notaries** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-public-services-post-banks-notaries` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Public Services: Post, Banks, Notaries** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-public-services-post-banks-notaries": {
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
