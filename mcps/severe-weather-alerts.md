# Severe Weather Alerts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/severe-weather-alerts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Active watches, warnings and advisories across the United States — NOAA NWS alerts by state, point or zone, with forecaster text, keyless.

## Description
Connect any AI agent to **official severe weather alerts for the United States** — the National Weather Service API that publishes every watch, warning and advisory in force right now. No key required.

### What you can do

- **See the national picture** — counts by event, severity, urgency and state, with the most severe alerts in force, from one request
- **List alerts in force** — ranked most severe first, paged, filterable by severity, urgency, event, state, latitude/longitude or UGC zone
- **Read one alert in full** — the forecaster's product text, the protective instructions, and the AWIPS and WMO product identifiers
- **Check a location** — every alert covering a latitude and longitude, with the forecast office responsible for it
- **Look up zones** — the forecast, county, fire and marine zones of a state, which is how alerts are tied to geography

### Why it matters

A warning is only useful if it reaches someone in time. Tornado Warnings carry urgency Immediate, Flood Watches are urgency Future, and the severity ranking puts Extreme and Severe events first. The feed also carries NWS system test messages — this server leaves them out unless asked, because they say "Monitoring message only, please disregard".


## Available Tools (5)
- **list_active_alerts**: Alert ids look like urn:oid:2.49... and are what get_alert_details takes. Feed entries that are system tests are left out unless include_tests is set — they say "Monitoring message only, please disregard".

List the weather watches, warnings and advisories in force right now — ranked most severe first, with event, severity, urgency, area, states and expiry for each, from NOAA NWS
- **summarize_active_alerts**: It reads the whole feed once and aggregates, so it costs one request instead of paging through hundreds of alerts. The by_state and by_event tables tell you which filter to pass to list_active_alerts next.

Summarise every weather alert in force across the United States right now — counts by event, severity, urgency and state, plus the most severe alerts in force, from NOAA NWS
- **get_alert_details**: id from list_active_alerts or summarize_active_alerts, or the full https URL of a single alert. Expired alerts are removed from the API, so an id that has ended returns "no alert exists" rather than a stale record — say so rather than retrying.

Read one weather alert in full — the forecaster's product text, the protective instructions, the area, the AWIPS and WMO product identifiers and the products it supersedes
- **get_alerts_at_point**: An empty answer means nothing is in force at that point. Coastal points may resolve to a marine zone, where Small Craft Advisories and Gale Warnings live.

Find every weather alert covering a latitude and longitude right now — what is in force exactly there, with the responsible NWS forecast office and zone
- **list_state_zones**: Counties are C codes (OHC009), forecast areas are Z codes (OHZ013).

List the NWS forecast, county, fire or marine zones of one US state, with the zone ids alerts attach to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Severe Weather Alerts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any weather alerts for my location at 39N, 77W?"

**🤖 AI Agent:**
> Nothing is in force at 39,-77 right now. That point falls in forecast zone MDZ504 under the NWS Sterling Virginia office (LWX), and no watch, warning or advisory covers it — that is a real clear result, not a failed lookup. When an alert does cover the point, it is matched against the alert polygon, which is more accurate than filtering by state.

---

**👤 You:**
> "What does the current Flood Warning for Minnesota say?"

**🤖 AI Agent:**
> Flood Warning FLSARX (WMO identifier WGUS83 KARX 192032), issued by NWS La Crosse Wisconsin for Mower County, Minnesota — severity Severe, urgency Expected, in force from September 19 at 3:32 PM CDT until September 21 at 3:32 AM CDT. It carries a polygon, so it can be matched to a point. The full product text is available by passing its id, urn:oid:2.49.0.1.840.0.[REDACTED].002.1, to get_alert_details.

---

**👤 You:**
> "How active is the weather across the country right now?"

**🤖 AI Agent:**
> Most of the alerts in force at any moment are marine, not land: Small Craft Advisories and Gale Warnings over coastal waters usually outnumber everything else, which is why a nationwide count looks high while your inland state looks quiet. The summary reports counts by event, severity, urgency and state, and ranks severity Extreme then Severe first — Flood Watches and Flood Warnings are the typical inland Severe events, with urgency Expected or Immediate. Call list_active_alerts with your state, or get_alerts_at_point with a latitude and longitude, to see only what covers you.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads the public National Weather Service API at api.weather.gov, which requires no key or account.

**Q: What is the difference between severity and urgency?**
Severity grades the phenomenon itself — Extreme and Severe mean threat to life and property. Urgency grades how soon it matters: Immediate means act now, Expected means within a few hours, Future means well ahead. A Tornado Warning is severity Severe and urgency Immediate; a Flood Watch is typically severity Moderate and urgency Future. Results are ranked by severity first, then urgency.

**Q: Why are some alerts missing from the results?**
The feed carries NWS system test messages that say "Monitoring message only. Please disregard." They are filtered out unless include_tests is set. Marine alerts — Small Craft Advisories, Gale Warnings — are genuine weather products and are always included; ask for a coastal point or a marine zone to see them.

**Q: Why did an alert id stop working?**
An alert is removed from the API once it ends, so an id from an earlier call returns "no alert exists" rather than a stale record. List the alerts again to get the ids currently in force — the same alert may also have been reissued with a new id and an Update message type.

**Q: Can I filter to more than one place at once?**
No — the NWS API rejects a request that carries both a state, a point and a zone. Choose one of them per call. To see alerts across several states, call summarize_active_alerts without a geographic filter and read the by_state table.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/severe-weather-alerts](https://vinkius.com/en/ai-agent-connect/severe-weather-alerts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Severe Weather Alerts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `severe-weather-alerts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Severe Weather Alerts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "severe-weather-alerts": {
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
