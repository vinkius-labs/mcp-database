# Route4Me MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/route4me)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/route4me-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/route4me-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Connect your AI assistant to Route4Me to orchestrate complex fleet logistics, solve multi-stop route optimizations, and track real-time vehicle GPS directly via chat.

## Description
Connect your conversational assistant directly to **Route4Me**, the global leader in dynamic route optimization and fleet management software. This integration effectively transforms your AI into an advanced automated dispatcher, empowering you to solve complex multi-stop delivery routes, monitor live GPS telematics, and adjust driver manifestations directly through seamless conversational commands.

### What you can do

- **Solve Complex Routes** — Ask your assistant to calculate optimal navigational paths (`create_optimization_problem`) minimizing fuel and time, or browse through historically solved logistics clusters (`list_optimizations`).
- **Manage Dispatched Fleet** — Instantly review all active trips (`list_dispatched_routes`) and pull a granular breakdown of stops and ETAs for any specific assigned path (`get_route_manifest`).
- **Real-Time GPS & Adjustments** — Query live vehicular telemetry (`get_route_gps_tracking`) on the fly, or inject unexpected new deliveries into an active driver's day log (`insert_stop_into_route`) without needing full re-optimizations.
- **Geocoding & Intelligence** — Provide the AI with rough address strings and have it instantly convert them into precise geographic mapping coordinates (`geocode_address`).

### How it works

1. Successfully attach the Route4Me logistics module to your active MCP ecosystem.
2. Sign in to your route planner dashboard with sufficient administrative or dispatch permissions. Seek out your centralized Account Settings to reveal your secure developer interface key.
3. Transcribe your unique `Route4Me API Key` strictly into the locked configuration matrix below.
4. Interface naturally with the logistics AI: "Show me the active delivery manifest for Route ID X, and give me the real-time GPS ping of the assigned truck."

### Who is this for?

- **Fleet Owners & Dispatchers** — Stop wrestling with spreadsheets and rigid software. Just verbally order the AI to inject a new priority stop into Driver B's current route.
- **Operations Managers** — Maintain a bird's-eye view using the AI to query real-time vehicle mapping and exact historical ETAs for failed deliveries entirely within your company chat.
- **Logistics Engineers** — Rapidly geocode large arrays of raw consumer address data dynamically for integration using intuitive AI textual pipelines.


## Available Tools
- **create_optimization_problem**: Provide a JSON object with parameters and addresses.

Creates a new route optimization problem
- **delete_dispatched_route**: This action is irreversible.

Deletes a dispatched route
- **geocode_address**: Converts a freeform address string into geographic coordinates
- **get_optimization_problem**: Retrieves details for a specific route optimization problem
- **get_route_gps_tracking**: Retrieves real-time or historical GPS tracking data for a route
- **get_route_manifest**: Retrieves the manifest (list of stops) for a specific route
- **insert_stop_into_route**: Inserts a new stop into an existing route
- **list_dispatched_routes**: Lists all dispatched routes
- **list_fleet_vehicles**: Lists all vehicles registered in the account
- **list_optimizations**: Lists historical and active route optimization problems


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Route4Me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the recently dispatched deliveries today."

**🤖 AI Agent:**
> I requested the dispatched lines pulling from `list_dispatched_routes` actively running through the system right now. Your dashboard indicates 3 live operational path allocations containing total multi-stop parameters. Let me know if you would like to drill down into a particular Route ID to see estimated times or locations manually.

---

**👤 You:**
> "Bring me the ETA and all address details for route '8B9A64'."

**🤖 AI Agent:**
> I requested the specific navigational matrix via `get_route_manifest` exclusively mapping to path '8B9A64'. The response contains 5 progressive destinations. Your requested vehicle has completed block 1, passing Main Street. Below is its progressive ETA log structure breaking down the following 4 remaining geographical nodes including targeted contact mapping details efficiently parsed:

---

**👤 You:**
> "Please geocode the location '123 Main St, New York, NY, 10001'."

**🤖 AI Agent:**
> I submitted the textual string through the `geocode_address` algorithmic logic. It precisely matched the parameter converting it effectively into verifiable numerical tracking values. Your coordinates output confirms standard positioning: Latitude 40.750, Longitude -73.996.


## Installation & Usage

To install and use the **Route4Me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/route4me](https://vinkius.com/mcp/route4me)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
