# Arcsecond.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcsecondio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access astronomical data and manage observatories with Arcsecond.io — search objects and track night logs via AI.

## Description
The **Arcsecond.io MCP Server** provides a unified natural language interface to the world's astronomical data. Connect your Arcsecond account to your AI agent to search for celestial objects, manage observatory data, and track observation night logs seamlessly.

### Key Features

- **Celestial Object Search** — Search for stars, galaxies, planets, and more to retrieve official names, types, and precise coordinates (RA/Dec).
- **Object Metadata** — Access detailed astrophysical data, including visual magnitude and classifications for millions of objects.
- **Observatory Management** — List observing sites, telescopes, and instruments associated with your observatory subdomain.
- **Data Tracking** — Access datasets and night logs to monitor ongoing observations and historical data collections.
- **Night Log Oversight** — Retrieve detailed logs of observations and calibrations organized by local noon-to-noon cycles.
- **Global Data Access** — Interface with a vast network of astronomical databases through a single, consistent API.

### Who is this for?

- **Professional Astronomers** — Quickly retrieve object coordinates and check observatory status without manual database queries.
- **Amateur Stargazers** — Search for interesting celestial targets and get detailed metadata for planning observation sessions.
- **Data Scientists** — Integrate astronomical data retrieval into automated research and analysis workflows.


## Available Tools (7)
- **get_account_check**: Verify Arcsecond account connection
- **get_object**: Get details for a specific astronomical object
- **list_datasets**: List datasets available for an observatory
- **list_night_logs**: List observation night logs for an observatory
- **list_observing_sites**: List observing sites for an observatory
- **list_telescopes**: List telescopes for an observatory
- **search_objects**: Search for astronomical objects (stars, galaxies, planets)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arcsecond.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the 'Andromeda Galaxy' and get its coordinates."

**🤖 AI Agent:**
> I've found the Andromeda Galaxy (M31). Its coordinates are RA: 00h 42m 44s, Dec: +41° 16′ 09″.

---

**👤 You:**
> "List all observing sites for the 'lco' observatory."

**🤖 AI Agent:**
> The LCO observatory has several sites, including McDonald Observatory (Texas), Cerro Tololo (Chile), and Siding Spring (Australia).

---

**👤 You:**
> "Show me recent night logs for subdomain 'my-observatory'."

**🤖 AI Agent:**
> I've retrieved the latest 5 night logs for 'my-observatory'. The most recent log from last night contains 15 successful observations and 3 calibration frames.


## ❓ FAQ

**Q: How do I get my Arcsecond.io API Key?**
Log in to your Arcsecond.io account and go to your **Profile** page. You will find your Personal API Key there.

**Q: What is an observatory subdomain?**
If you are part of a specific observatory or organization on Arcsecond.io, your data is hosted on a subdomain (e.g., `myobs.arcsecond.io`). You can use this subdomain to access site-specific data.

**Q: Can I search for any astronomical object?**
Yes, the `search_objects` tool allows you to search across millions of objects in the SIMBAD, Gaia, and other astronomical databases integrated into Arcsecond.io.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcsecondio](https://vinkius.com/mcp/arcsecondio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arcsecond.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arcsecondio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arcsecond.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arcsecondio": {
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
