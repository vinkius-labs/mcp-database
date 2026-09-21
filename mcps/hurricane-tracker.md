# Hurricane Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hurricane-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Active tropical cyclones and official NHC forecast tracks — position, wind, pressure, the five-day track with wind radii, and the Tropical Weather Outlook, keyless.

## Description
Connect any AI agent to **NOAA's National Hurricane Center** — the official source for Atlantic and Pacific tropical cyclone forecasts. No key required.

### What you can do

- **List every active storm** — depressions, tropical storms and hurricanes, with classification, wind speed, pressure, position and movement
- **Read the official forecast track** — the newest forecast/advisory product, parsed into a table of positions, maximum wind and gusts at each forecast time, plus the 34/50/64-knot wind radii
- **Read the Tropical Weather Outlook** — the forecaster discussion of disturbances and their chances of developing over the next two to seven days
- **Translate a place into a basin** — the Gulf of Mexico and Caribbean are the Atlantic (AT), the Pacific off Mexico is EP, the waters around Hawaii are CP

### Why it matters

Every other weather source paraphrases the NHC. This reads the actual WMO forecast/advisory product, so the answer carries the forecaster's own radii, gusts and confidence — the numbers emergency managers plan against.


## Available Tools (4)
- **get_storm_forecast**: Wind radii are the largest radius in nautical miles where that wind strength is expected somewhere in that quadrant. Points marked "outlook" are the day 4–5 extended forecast with larger errors; a state of "POST-TROP/REMNT LOW" or "DISSIPATED" means the storm is forecast to lose tropical characteristics, not that a position exists. Throws when the storm is too weak for an advisory.

Get the official NHC forecast track for one active tropical cyclone — the five-day positions, maximum wind and gusts at each forecast time, the 34/50/64-knot wind radii, and when the next advisory is due
- **get_tropical_outlook**: Basins: AT (Atlantic, Gulf and Caribbean), EP (eastern Pacific off Mexico) and CP (central Pacific around Hawaii). The text is a verbatim WMO product, quoted as a block.

Read the plain-text Tropical Weather Outlook for a basin — the NHC forecaster discussion of disturbances that could develop into tropical cyclones over the next two to seven days
- **list_tropical_basins**: List the tropical cyclone basins NHC publishes outlooks for, with what each one covers
- **list_active_storms**: The list is the NHC official active-storm summary and refreshes several times a day. When the answer is empty, there really is nothing active — do not retry, suggest the Tropical Weather Outlook instead. The id (e.g. al062026) is what the other tools take; a name like "Six" also works once this list has been loaded.

List every active tropical depression, tropical storm and hurricane in the Atlantic and eastern Pacific right now — name, id, classification, wind speed, pressure, position and movement, from NOAA NHC


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hurricane Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there any hurricane active right now?"

**🤖 AI Agent:**
> No tropical cyclone is active in the Atlantic or eastern Pacific at the moment — the NHC active-storm list is empty. The Atlantic Tropical Weather Outlook is tracking one tropical wave with a 20 percent chance of development over the next five days.

---

**👤 You:**
> "Where will Tropical Storm Six be in three days, and how strong?"

**🤖 AI Agent:**
> Per NHC forecast/advisory number 3, issued 0300 UTC Sep 20: Tropical Depression Six is at 33.3N 33.2W with 30 kt winds, moving north-northeast at 4 kt. By 21/1200Z it is forecast near 33.6N 32.4W at 40 kt, and by 23/0000Z near 30.4N 35.6W, weakened to a 25-kt post-tropical remnant low. Next advisory at 20/0900Z.

---

**👤 You:**
> "Aside from Six, is anything else brewing in the Atlantic? What's the tropical outlook for the coming week?"

**🤖 AI Agent:**
> The Atlantic Tropical Weather Outlook issued at 200 AM EDT Sun Sep 20 2026 (forecaster Cangialosi) names only one active system — Tropical Depression Six, several hundred miles southwest of the Azores — and states plainly that tropical cyclone formation is not expected during the next 7 days anywhere in the basin. Advisory headers for Six: public advisories under WMO header WTNT31 KNHC (AWIPS MIATCPAT1), forecast/advisories under WTNT21 KNHC (AWIPS MIATCMAT1).


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads the National Hurricane Center's public website, which requires no key or account.

**Q: What does it mean when the list is empty?**
There genuinely is no active tropical cyclone in the Atlantic or eastern Pacific at that moment. The list is not a forecast — call get_tropical_outlook to see the disturbances NHC is watching for possible development instead.

**Q: Why does a forecast point have no position?**
A point whose state reads POST-TROP/REMNT LOW or DISSIPATED is a forecast of the storm losing tropical characteristics, not a place to plot. Points marked "outlook" are the day 4–5 extended forecast, which carries larger errors than the first three days.

**Q: How fresh is the forecast track?**
The tool always reads the newest advisory published for that storm — advisories are issued every six hours when a storm is active, and the response says when the next one is due.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hurricane-tracker](https://vinkius.com/en/ai-agent-connect/hurricane-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hurricane Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hurricane-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hurricane Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hurricane-tracker": {
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
