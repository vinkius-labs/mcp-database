# Volcano Activity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/volcano-activity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

The Smithsonian / USGS Weekly Volcanic Activity Report as structured data — which volcanoes erupted this week, where, at what alert level, and how far the exclusion zone reaches. Keyless.

## Description
Connect any AI agent to the **Smithsonian Global Volcanism Program / USGS Weekly Volcanic Activity Report** — the authoritative weekly summary of volcanic unrest and eruption worldwide, published every Thursday by 2300 UTC. No key required.

### What you can do

- **Take the global pulse** — how many volcanoes are reported this week, which countries they are in, how many began erupting or showed new unrest, and the highest alert levels, ash plumes and exclusion zones in the report
- **List the active volcanoes** — every entry with its position, activity type, alert level, ash plume height and exclusion zone, filterable by type, country, name and area
- **See only what is new** — the eruptions and unrest that began this week, rather than the continuing ones
- **Check your own area** — volcanoes with notable activity within a radius of any point on Earth, nearest first
- **Read one full report** — the complete scientist-written narrative, the observatory that filed it and its sources

### Why it matters

A volcano's alert level and exclusion zone are the two numbers that decide whether a place is safe. The report carries them in scientists' own prose, alongside the observatory that measured them — PVMBG for Indonesia, JMA for Japan, PHIVOLCS for the Philippines — so an answer can name its authority rather than assert a risk.

The report is a summary of activity that met selected criteria. It is not a complete list of every eruption on Earth, and it lists roughly twenty volcanoes a week — so an empty result for a region usually means nothing notable is active there, not missing data.


## Available Tools (5)
- **get_volcano_report**: Only volcanoes in the current week's report can be returned; when the name is unknown the error lists every volcano this week's report does cover, so read it and retry. The body is the report as published — quote it rather than paraphrasing it, and name the observatory in the Sources list as the authority. Alert level, ash plume and exclusion zone are read out of prose: treat them as a reading aid and check them against the body before acting on them.

The full weekly report for one volcano — the complete scientist-written narrative, its sources, the reporting observatory and whatever alert level, ash plume height and exclusion zone the text states
- **list_active_volcanoes**: Filters combine: activity_type (New Eruptive Activity, Continuing Eruptive Activity, New Unrest, Continuing Unrest, Other Observations), country (matched loosely, accents folded), free text q on the volcano name or its Smithsonian number, and bounding_box as south,west,north,east. Results are paged: defaults give 25 from offset 0 and has_more says whether to ask again with a higher offset. New activity sorts first. Alert levels, ash plume heights and exclusion zones are extracted from the report prose and may be absent for a given volcano — the summary field always has the human-written lead sentence.

List the volcanoes in this week's report — name, country, activity type, position, alert level, ash plume height and exclusion zone, filterable by type, country, text and area
- **find_volcanoes_nearby**: Give latitude and longitude in decimal degrees and radius_km (default 100, capped at 2000). An empty answer is the normal result for most of the planet: the report lists only about twenty volcanoes a week worldwide, so absence means nothing notable is active there, not missing data. Widen radius_km before concluding nothing is nearby. Results are paged with offset and amount.

Volcanoes with notable activity within a radius of any point on Earth — nearest first, with distance in kilometres
- **list_new_activity**: country, free text q and bounding_box all narrow it further, and results are paged with offset and amount. When this list is empty, nothing new began: the week's activity is all continuing.

Only the volcanoes whose activity is NEW this week — new eruptions and new unrest. These are the reports that change the situation rather than describe a continuing one
- **get_report_summary**: This is the Smithsonian / USGS Weekly Volcanic Activity Report, published every Thursday by 2300 UTC: it summarises activity that met selected criteria and is NOT a complete list of every eruption on Earth — say so when you report it. Optionally pass a bounding_box to count only one region. Alert levels, ash heights and exclusion zones are read out of scientists' free prose and may be missing; the per-volcano reports carry the full text.

The state of volcanic activity worldwide this week — how many volcanoes are reported, which countries they are in, how many began erupting or showed new unrest, and the highest alert levels, ash plumes and exclusion zones in the report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volcano Activity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Did any new volcano eruptions start this week?"

**🤖 AI Agent:**
> One volcano began new eruptive activity in the report for 10–16 September 2026: Krakatau in Indonesia. PVMBG, the Indonesian volcano observatory, reported fourteen Strombolian eruptions during 6–11 September, with an ash plume reaching 2.1 km above the summit on the 9th as analysed in a Himawari-9 satellite image. The alert level stands at 3 on Indonesia's 1–4 scale and the public is advised to stay 3 km from the summit. Beyond that, eighteen volcanoes are reported as continuing eruptive activity — most of them in Indonesia and Russia — and one entry records a lowered alert level. So the week's change is concentrated at Krakatau.

---

**👤 You:**
> "I'm planning a trip to Bali. Is there any volcano activity I should worry about nearby?"

**🤖 AI Agent:**
> Searching within 300 km of Bali, the current Weekly Volcanic Activity Report lists no volcano with notable activity in that radius — so the report's roughly twenty entries this week are all elsewhere, and there is no elevated activity being reported for the region. That is a meaningful answer about this week's notable activity, not a guarantee of safety: Bali sits on the Ring of Fire and its volcanoes are monitored continuously by PVMBG. For a travel decision, check the current PVMBG advisories for Mount Agung and Mount Batur directly, and register with your embassy's volcano alert service if your government offers one.

---

**👤 You:**
> "Give me the full report on Mount Merapi."

**🤖 AI Agent:**
> Merapi, on the border of Central Java and Yogyakarta in Indonesia, appears in this week's report as continuing eruptive activity. The alert level stands at 3 on Indonesia's four-level scale — the second-highest tier — with the public warned to stay at least 5 km from the Jonggring Seloko crater, and further out on the southeast flank where pyroclastic flows have travelled in past crises. PVMBG is the reporting authority, and the report also notes the dome growth and avalanche events that kept the level at 3. For the exact figure on any given day, the PVMBG advisory is the primary source; this report is the weekly digest of what the observatory observed.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads the public GeoRSS feed of the Smithsonian / USGS Weekly Volcanic Activity Report, which requires no key or account.

**Q: Is this a complete list of every erupting volcano?**
No, and the source says so itself. The Weekly Volcanic Activity Report summarises activity that met selected criteria — significant new eruptions, changes in alert level, or notable ongoing activity. It typically lists around twenty volcanoes a week out of the roughly 1,300 that have erupted in historical time, so treat it as the authoritative digest of what changed, not an exhaustive catalogue.

**Q: Why is the alert level missing for some volcanoes?**
Alert levels are written in free prose by the reporting observatory, and each country words them differently — some reports state no numeric level at all. The tool reads them out of the text where they are stated and leaves the field empty where they are not; the full report body is always returned alongside so nothing is hidden. Check the body before acting on any extracted number.

**Q: How fresh is the data?**
The report is published every Thursday by 2300 UTC, so on a Thursday or Friday you are reading the freshest issue; later in the week you are reading the previous Thursday's report. Each answer carries its own report window and publication timestamp — quote those alongside any figure so the reader knows which week it describes.

**Q: Why does find_volcanoes_nearby return nothing for my location?**
Because nothing notable is active there. The report lists only about twenty volcanoes a week worldwide, so for most of the planet — including all of Europe outside Iceland and Italy — the answer is genuinely empty. Increase radius_km before concluding the search is broken; the radius caps at 2,000 km.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/volcano-activity](https://vinkius.com/en/ai-agent-connect/volcano-activity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volcano Activity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `volcano-activity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volcano Activity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volcano-activity": {
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
