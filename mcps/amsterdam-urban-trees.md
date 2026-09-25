# Amsterdam Urban Trees MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-urban-trees)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless access to Amsterdam's urban tree registry: individual trees (species, height, planting year), storm damage reports, safety inspections and felling/replanting records — the city's open-data platform, no API key.

## Description
Amsterdam's complete tree registry, keyless. The city manages every public tree in its inventory; this integration exposes that registry plus the operational records around it.

### What you can do
- **Tree inventory** — search individual trees by species (e.g. Tilia americana), neighbourhood, location type or height class; each with planting year, owner/manager and point geometry
- **Storm damage reports** — tree damage registered under named storms (Conall, Lothar, Kyrill), with damage type and closest address
- **Safety inspections** — tree safety inspection records (BVO), inspecting organisation and pruning method
- **Removal & replanting** — felling permits and replanting decisions with defects, dates and tree details

### Who is this for
Urban foresters, researchers, property owners checking the trees on their street, and agents that reason about green infrastructure or storm risk.


## Available Tools (5)
- **search_trees**: Filter by species or neighbourhood to see which trees are planted where.

Search the city tree inventory (bomen)
- **get_tree**: Get one tree record by id
- **list_storm_reports**: g. Conall, Lothar, Kyrill): damage type, closest address, report date and time, neighbourhood, storm name and whether the storm is currently active.

List storm damage reports on trees
- **list_safety_inspections**: g. Boomveiligheidsonderhoud / BVO), inspecting organisation, inspection date, object start time and pruning method. Filter by tree id to see the inspection history of one tree.

List tree safety inspections
- **list_tree_removal_records**: g. felling), dates of the permit process, species, trunk diameter, neighbourhood and point geometry.

List tree felling and replanting decisions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Urban Trees** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many American elms (Tilia americana) are in the tree registry?"

**🤖 AI Agent:**
> 🌳 **Tree search**

search_trees filtered by species "Tilia americana" returns the matching trees, each with its height class, planting year, owner and point geometry (EPSG:28999), plus the pagination total.

---

**👤 You:**
> "Show the tree storm damage reports from the Conall storm."

**🤖 AI Agent:**
> list_storm_reports filtered by storm name returns the reports: damage type (e.g. "04 - Afgebroken takken" = broken branches), closest address, report date, neighbourhood and whether the storm is still active.

---

**👤 You:**
> "What is the safety inspection history of tree 921115?"

**🤖 AI Agent:**
> list_safety_inspections filtered by tree id returns the inspection records: inspection type (e.g. Boomveiligheidsonderhoud / BVO), inspecting organisation, inspection date and pruning method.


## ❓ FAQ

**Q: Do I need an API key?**
No. The bomen v2 service of the city's DSO open-data platform is public (OPENBAAR) and works with zero credentials.

**Q: What is in a tree record?**
Each stamgegevens record carries the species name, height class, trunk diameter class, planting year, owner and manager, where the tree stands, its protection status and a point location in EPSG:28999 (RD New).

**Q: Can I check whether a specific tree was inspected?**
Yes. Pass the tree id to list_safety_inspections to see its inspection history (type, organisation, date, pruning method). The same id works with list_tree_removal_records to check felling/replanting decisions.

**Q: Which storms have damage reports?**
Storm damage reports are registered under named storms such as Conall (2024/25). Filter list_storm_reports by the storm name, or by active=true to see damage from a storm currently in progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-urban-trees](https://vinkius.com/en/ai-agent-connect/amsterdam-urban-trees)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Urban Trees** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-urban-trees` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Urban Trees** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-urban-trees": {
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
