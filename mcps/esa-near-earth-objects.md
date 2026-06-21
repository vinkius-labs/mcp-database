# ESA Near Earth Objects MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esa-near-earth-objects)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Track near-Earth asteroids and comets, access orbital data, and monitor potential impact risks from the European Space Agency.

## Description
Connect to the **European Space Agency Near-Earth Object Coordination Centre (NEOCC)** and access the most authoritative asteroid monitoring data in Europe.

### What you can do

- **Close Approaches** — Retrieve upcoming and recent asteroid flybys with miss distances in kilometers, astronomical units, and lunar distances, plus diameter and relative velocity
- **Impact Risk Assessment** — Access the official ESA risk list and special risk list of asteroids with non-zero cumulative impact probability, including Palermo Scale and Torino Scale ratings
- **Object-Level Intelligence** — Query orbital elements, physical properties (diameter, albedo, spectral type), and computed ephemerides for any known near-Earth object by designation
- **Planetary Defence Monitoring** — Access the Aegis impact monitoring table and priority observation lists used by ESA Space Safety

### How it works

1. Subscribe to this server
2. No API key required — the ESA NEOCC is a public service
3. Start querying asteroid data from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a planetary defence analyst with direct access to ESA mission-critical data. All information is sourced from the ESA Space Safety programme and updated multiple times daily.

### Who is this for?

- **Researchers & Astronomers** — access orbital elements and ephemerides for observation planning without navigating complex web portals
- **Science Communicators** — instantly retrieve upcoming asteroid flyby data for articles and social media
- **Planetary Defence Professionals** — monitor risk lists and impact tables programmatically for rapid response workflows
- **Space Enthusiasts** — explore the asteroid catalog and track objects approaching Earth in near real-time


## Available Tools
- **check_esa_neocc_status**: Returns the connection status and service URL. Use this to verify the integration is working correctly.

Verify ESA NEOCC API connectivity
- **get_all_nea_list**: Returns designations only. Warning: this list contains thousands of entries. Use for comprehensive audits or when searching for a specific designation.

Get the complete catalog of all known near-Earth asteroids
- **get_impact_table**: Lists virtual impactors with their projected impact dates, impact probabilities, and Palermo Scale values. This is the primary ESA output for planetary defence risk assessment.

Get impact monitoring data for potentially hazardous objects
- **get_object_close_approaches**: g., "2024YR4", "99942 Apophis"). Returns miss distance, date, velocity, and brightness for each encounter. Use URL-encoded designations for objects with spaces.

Get all close approaches for a specific asteroid
- **get_object_ephemerides**: Returns right ascension, declination, distance, and visual magnitude at each timestep. Useful for planning telescope observations or determining current sky position.

Get ephemerides for a specific asteroid
- **get_object_orbital_elements**: Essential for trajectory computation and impact probability assessment.

Get orbital elements for a specific asteroid
- **get_object_physical_properties**: Data sourced from the ESA NEOCC physical properties database.

Get physical properties of a specific asteroid
- **get_priority_list**: These objects have incomplete orbital arcs and could be reclassified with additional tracking data.

Get priority NEOs requiring follow-up observation
- **get_recent_close_approaches**: Useful for reviewing past flyby events and validating orbital predictions.

Get recent asteroid close approaches that already occurred
- **get_risk_list**: Each entry includes the object designation, estimated diameter, cumulative impact probability (IP), Palermo Scale value (PS), and Torino Scale rating. Objects on this list are being actively monitored by the ESA Planetary Defence Office.

Get the ESA asteroid impact risk list
- **get_special_risk_list**: These objects have heightened scientific interest for planetary defence.

Get the ESA special priority risk list
- **get_upcoming_close_approaches**: Data is updated multiple times per day directly from the ESA Space Safety programme.

Get upcoming asteroid close approaches to Earth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ESA Near Earth Objects** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all asteroids approaching Earth in the next few months."

**🤖 AI Agent:**
> I've retrieved the ESA NEOCC upcoming close approaches list. There are currently 87 objects tracked. The closest approach today is asteroid 2022UU8, passing at 3.34 million km (8.7 lunar distances) with a diameter of approximately 9 meters. Would you like me to check the risk assessment for any of these objects?

---

**👤 You:**
> "Are there any asteroids currently on the ESA risk list?"

**🤖 AI Agent:**
> I've fetched the ESA risk list. There are currently several objects with non-zero cumulative impact probability. The highest-rated object has a Palermo Scale value of -2.3 and Torino Scale 0. None currently warrant public concern — all are within normal background risk levels. Would you like the orbital details for any specific object?

---

**👤 You:**
> "Get me the orbital elements and physical properties of asteroid 2024YR4."

**🤖 AI Agent:**
> Querying the NEOCC database for 2024YR4... The orbital elements show a semi-major axis of 1.47 AU, eccentricity 0.42, inclination 3.8°. The physical properties indicate an estimated diameter of 40-90 meters with absolute magnitude H=24.7. This object was flagged for follow-up observations. Would you like to see its computed ephemerides for telescope planning?


## ❓ FAQ

**Q: Do I need an API key to use this server?**
No. The ESA NEOCC API is completely public and requires no authentication. Simply subscribe to this server and enter any placeholder value in the API key field to start querying asteroid data immediately.

**Q: How often is the asteroid data updated?**
The ESA NEOCC updates its close approach data, risk lists, and impact monitoring tables multiple times per day. Orbital elements and physical properties are updated whenever new observational data becomes available from ground-based telescopes worldwide.

**Q: Can I query data for a specific asteroid like Apophis?**
Yes! Use the object-specific tools with the asteroid's designation. For example, query orbital elements for '99942' (Apophis), or get close approaches for '2024YR4'. The designation should match the official IAU format used in the NEOCC database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esa-near-earth-objects](https://vinkius.com/mcp/esa-near-earth-objects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ESA Near Earth Objects** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `esa-near-earth-objects` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ESA Near Earth Objects** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "esa-near-earth-objects": {
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
