# ESA Near Earth Objects MCP Server

Track near-Earth asteroids and comets, access orbital data, and monitor potential impact risks from the European Space Agency.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/esa-near-earth-objects)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

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


## Installation & Usage

To install and use the **ESA Near Earth Objects** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esa-near-earth-objects](https://vinkius.com/mcp/esa-near-earth-objects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
