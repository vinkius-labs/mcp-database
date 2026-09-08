# Space Launches & Astronauts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/space-launches-astronauts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Every rocket launch on Earth, as an MCP: upcoming and past launches (SpaceX, NASA, Roscosmos, CASC...), astronauts in orbit, agencies, rocket specs — Launch Library 2, anonymous or with API token for high rate limits.

## Description
**The global spaceflight registry** (Launch Library 2 by The Space Devs) as a single MCP server — every orbital launch attempt on Earth, past and future.

### What you can do
- **Upcoming launches** — live schedules with "Go for Launch" status, launch windows, provider, rocket, orbit, pad (Baikonur, Cape Canaveral, Wenchang...) and live-webcast flags
- **Launch history** — outcomes with failure reasons; thousands of launches searchable by name ("Starship", "Artemis", "Soyuz")
- **Astronauts** — profiles with flight counts, spacewalk hours, birthdates and the **in_space=true** filter: who is in orbit right now
- **Agencies & rockets** — NASA (id 44), SpaceX (121), Roscosmos (63)... with launch stats; 532 rocket configurations with specs (thrust, payload to LEO, stages)
- **Optional API token** — anonymous access works out of the box (~15 req/h); add a free thespacedevs.com token in the credentials tab to unlock 1000+ req/h

### Why it matters
Spaceflight is mainstream now: Starship test flights, Artemis, Chinese megaconstellations. This MCP gives agents the authoritative live schedule and history — no scraping news sites.

### Who is this for?
Space content creators, news monitoring, developers building launch-notification apps, researchers, and anyone whose agent should know that a Falcon 9 just lifted off.


## Available Tools (7)
- **get_next_launches**: Supports LSP id filtering (e.g. 121 = SpaceX). Offset/limit pagination — the API has thousands of scheduled launches.

Get the next upcoming rocket launches worldwide (SpaceX, NASA, Roscosmos, CASC...)
- **get_past_launches**: Use for "did that launch succeed?" and launch-rate research.

Get past rocket launches with outcomes (success/failure reasons)
- **search_launches**: Returns the same launch details as get_next_launches — works for both upcoming and historical launches.

Search launches by name or mission (e.g. "Artemis", "Starship", "Falcon 9")
- **get_launch_details**: Use ids from other launch tools.

Get every detail of ONE launch by id: mission, rocket config, pad, window, probability, streams
- **get_astronauts**: Filter is_human=true to exclude animals. Great for "who is currently in orbit?".

Search astronauts: who is in space right now, flight counts, agencies
- **get_space_agency**: Use agencies seen in launch data.

Get details of a space agency: launch stats, founded, description, spacecraft
- **search_rockets**: g. "Falcon 9", "Starship", "Soyuz", "Ariane"): full_name, family, maiden_flight, payload capacity, thrust, height, stages. The reference tool for rocket-spec questions.

Browse rocket configurations (532 rockets): families, maiden flights, thrust, payload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Space Launches & Astronauts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the next rocket launch and can I watch it live?"

**🤖 AI Agent:**
> 🚀 **Next launch**

**Progress MS-35 (96P)** — Soyuz 2.1b, ROSCOSMOS
- Status: **Go for Launch**
- Window: 2026-09-09 16:15 UTC
- Pad: Baikonur Cosmodrome, Kazakhstan
- Orbit: Low Earth Orbit (ISS resupply)

Webcast link included in the data. Two more launches within the next 48h — want the full week schedule?

---

**👤 You:**
> "Who is in space right now?"

**🤖 AI Agent:**
> 👨‍🚀 **Astronauts currently in orbit (in_space=true)**

- NASA crew members aboard ISS Expedition (flights 2-4 each)
- Roscosmos cosmonauts with 300+ days cumulative
- Spacewalk totals pulled from EVA records

I can pull any astronaut's full profile — bio, agency, mission history.

---

**👤 You:**
> "Specs of the Falcon 9 — payload, thrust, first flight"

**🤖 AI Agent:**
> 🛰️ **Falcon 9 (SpaceX, config from LL2)**

- Family: Falcon
- Maiden flight: 2010-06-04
- Payload to LEO: ~22,800 kg (full data in the response)
- Stages: 2 (+ booster reuse)

I can compare with Electron, Vulcan or list every Falcon 9 launch ever — there are hundreds.


## ❓ FAQ

**Q: Do I need an API key?**
Not necessarily: anonymous access works immediately (about 15 requests/hour). For heavier use, register free at thespacedevs.com and paste the token into the MCP's credentials tab — it unlocks 1000+ requests/hour.

**Q: Does this cover only SpaceX?**
No — it covers every orbital launch attempt worldwide: SpaceX (121), NASA (44), Roscosmos (63), CASC, ISRO, Rocket Lab, Arianespace and 100+ more agencies, plus thousands of historical launches since 1957.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/space-launches-astronauts](https://vinkius.com/ai-agent-connect/space-launches-astronauts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Space Launches & Astronauts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `space-launches-astronauts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Space Launches & Astronauts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "space-launches-astronauts": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
