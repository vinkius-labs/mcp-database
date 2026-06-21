# Shovels MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shovels)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shovels-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shovels-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Construction and permit data platform — search contractors and building permits via AI.

## Description
Empower your AI agent to access the most comprehensive database of construction permits and licensed contractors with **Shovels**. By connecting Shovels to your agent, you transform complex real estate and construction auditing into a natural conversation. Your agent can instantly search for active permits, audit contractor history, and retrieve market statistics for specific geographic areas without you ever touching a dashboard. Whether you are analyzing market trends or verifying contractor credentials, your agent acts as a real-time construction data analyst, ensuring your insights are always structured and up-to-date.

### What you can do

- **Contractor Discovery** — Find licensed professionals based on location, work type (solar, roofing, etc.), and property type.
- **Permit Auditing** — Search for and inspect detailed building permit records, including status and estimated values.
- **Activity Tracking** — Identify contractors actively working within a specific radius of any address.
- **Market Intelligence** — Retrieve aggregated permit statistics to analyze construction trends in different cities or counties.
- **License Verification** — Instantly pull contractor profiles using their state business license IDs.

### How it works

1. Subscribe to this server
2. Enter your Shovels.ai API Key
3. Start managing your construction data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Developers** — perform rapid due diligence on properties and track local development activity.
- **Market Researchers** — analyze construction trends and identify high-growth areas based on permit volumes.
- **Homeowners & Propert Managers** — verify contractor credentials and monitor work history in their neighborhood.
- **SaaS Developers** — integrate construction and permitting workflows into their applications through an AI-guided interface.
- **Building Material Suppliers** — identify active job sites and contractors to optimize sales outreach.


## Available Tools
- **get_contractor_activity**: Find contractors active at an address
- **get_contractor_by_license**: Find contractor by license ID
- **get_contractor**: Get contractor details
- **get_permit_stats**: Get permit activity statistics
- **get_permit**: Get permit details
- **search_contractors**: Search for licensed contractors
- **search_permits**: Search for building permits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shovels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for roofing contractors in ZIP 94105."

**🤖 AI Agent:**
> I've searched Shovels for roofing professionals in San Francisco (94105). I found 8 active contractors, including 'Bay Area Roofing' and 'Elite Home Exteriors'. Would you like to see their full credentials?

---

**👤 You:**
> "Show me permit stats for Austin, TX."

**🤖 AI Agent:**
> Retrieving permit activity for Austin... I see a 15% increase in residential remodeling permits this quarter, with a total of 1,200 active filings. I can break this down by permit type if needed.

---

**👤 You:**
> "Find contractors active near 1600 Amphitheatre Pkwy, Mountain View."

**🤖 AI Agent:**
> Scanning work activity near Googleplex... I've identified 12 contractors doing work within a 5-mile radius, mostly focusing on commercial HVAC and electrical upgrades. Shall I list the companies for you?


## Installation & Usage

To install and use the **Shovels** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shovels](https://vinkius.com/mcp/shovels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
