# Moscow Schools, Kindergartens & Universities MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-schools-kindergartens-universities)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Keyless Moscow education: schools, kindergartens, universities and colleges, language and driving schools, plus the Russian Wikipedia university roll.

## Description
The mapped education estate of the city, keyless — about 1,300 schools, 2,000 kindergartens and 300 universities and colleges, plus the supplementary-school layer.

### What you can do
- **find_schools** — general-education schools (about 1,300) filtered by name — gymnasiums, lyceums and ordinary schools — with operator and contacts
- **find_kindergartens** — kindergartens and pre-schools (about 2,000), the practical question being which are within walking distance
- **find_universities** — universities and colleges (about 300) — MSU on Sparrow Hills, the polytechnics, the smaller institutes — filtered by name
- **find_extra_schools** — language, driving, music, art and dance schools — pick one kind or take the full mix
- **universities_wiki** — the Russian Wikipedia roll of Moscow universities, with a short encyclopaedia entry for the first
- **education_profile** — citywide counts of schools, kindergartens, universities, colleges, libraries and extra schools in one call

### Who is this for
Families choosing a neighbourhood and comparing local schools, and anyone sizing the city’s education estate for a move or a report.


## Available Tools (6)
- **find_kindergartens**: Each row carries the name, operator, phone and coordinate. Filter by name fragment or narrow to a neighbourhood with lat/lon/km — the practical question is always "which kindergartens are within walking distance of this address".

Find Moscow kindergartens and pre-schools
- **education_profile**: Use it to size a district question without paging through lists. No filters — this is a profile, not a search.

Citywide Moscow education profile
- **find_extra_schools**: Pass kind to pick one ("language", "driving", "music", "art", "dance") or leave it out for the full mix. Each row carries the name, phone, website and coordinate.

Find Moscow language, driving, music and art schools
- **find_schools**: Each row carries the name, operator, phone, website and the centre coordinate. Filter by name fragment (e.g. "Гимназия", "Лицей", "1543") or find the schools around an address with lat/lon/km. For universities use find_universities; for pre-school use find_kindergartens.

Find Moscow schools
- **find_universities**: Each row carries the name, phone, website and coordinate. Filter by name fragment (e.g. "МГУ", "Политех") or narrow to a district with lat/lon/km. For the encyclopaedic roll of Moscow universities use universities_wiki.

Find Moscow universities and colleges
- **universities_wiki**: Useful when a name needs grounding ("is this a state university?") because the map tags carry no accreditation data. Pass detail: "true" to fetch the summary of the first listed university; otherwise the tool returns the plain title list.

Moscow university roll from Russian Wikipedia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Schools, Kindergartens & Universities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which kindergartens are within 2 km of this address?"

**🤖 AI Agent:**
> find_kindergartens with the address coordinates and km: "2" returns the mapped pre-schools with their distances.

---

**👤 You:**
> "Tell me about Moscow State University."

**🤖 AI Agent:**
> universities_wiki with detail: "true" returns the Wikipedia entry for the first listed university; find_universities with name: "МГУ" locates the campus on the map.

---

**👤 You:**
> "How many schools and kindergartens does Moscow have?"

**🤖 AI Agent:**
> education_profile returns the citywide counts in one call — the map records about 1,300 schools and 2,000 kindergartens.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: Do the tools cover admissions and exam scores?**
No. The map gives the estate itself — locations, names, operators, phones — and the Wikipedia roll gives the encyclopaedia entries. Admissions data lives on Moscow’s own portals, which refuse connections from outside Russia.

**Q: Why are the counts bigger than the rows I get?**
Yes. OSM maps most large venues as areas (stadiums, monastery enclosures, university campuses), and every list tool uses the nwr selector, so nodes, ways and relations all count.

**Q: Can I find schools near an address?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-schools-kindergartens-universities](https://vinkius.com/en/ai-agent-connect/moscow-schools-kindergartens-universities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Schools, Kindergartens & Universities** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-schools-kindergartens-universities` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Schools, Kindergartens & Universities** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-schools-kindergartens-universities": {
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
