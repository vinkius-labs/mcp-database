# Perenual Plant API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/perenual-plant-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage plant data — audit species, care, and diseases via AI.

## Description
Empower your AI agent to orchestrate your entire botanical research and plant auditing workflow with the **Perenual Plant API**, the comprehensive source for species-specific care data. By connecting Perenual to your agent, you transform complex plant searches into a natural conversation. Your agent can instantly identify plant species, audit watering and sunlight requirements, and query disease identification metadata without you ever touching a gardening portal. Whether you are conducting horticultural research or managing local greenhouse constraints, your agent acts as a real-time botanical consultant, ensuring your data is always verified and localized.

### What you can do

- **Species Auditing** — Search for thousands of plant species by common or scientific name and retrieve detailed metadata, including IDs and names.
- **Care Oversight** — Audit specific care guides for any species to understand watering, sunlight, and maintenance distribution instantly.
- **Disease Discovery** — Search for common plant pests and diseases to identify relevant biological markers for your greenhouse.
- **Horticultural Intelligence** — Retrieve high-resolution details for specific species IDs to assist in deep-dive botanical classification.
- **Operational Monitoring** — Check API status to ensure your botanical research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Perenual API Key
3. Start managing your botanical intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Horticulturists & Botanists** — monitor species data and retrieve official metadata straight from your workflow.
- **Greenhouse Managers** — verify care requirements and audit plant health patterns without manual searching.
- **Gardening Enthusiasts** — perform rapid audits of plant diseases and identify relevant care markers through natural language.
- **Operations Leads** — automate botanical data querying to orchestrate cross-functional agricultural teams smoothly.


## Available Tools
- **check_api_status**: Check if the Perenual service is operational
- **get_plant_care_guide**: Get care instructions and guides for a specific plant
- **get_plant_details**: Get full details for a specific plant by species ID
- **search_plant_diseases**: Search for common plant pests and diseases
- **search_plants**: Search for plants by common or scientific name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perenual Plant API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'monstera' using Perenual Plant API."

**🤖 AI Agent:**
> I've retrieved the data for Monstera! Multiple species are identified, including Monstera Deliciosa and Monstera Adansonii. Would you like the care requirements or species ID for any of these?

---

**👤 You:**
> "What is the care guide for species ID 5257?"

**🤖 AI Agent:**
> I've retrieved the care guide for ID 5257. It requires frequent watering and bright, indirect sunlight. I can provide the full maintenance breakdown and pruning metadata if you'd like.

---

**👤 You:**
> "Search for plant diseases related to 'root rot'."

**🤖 AI Agent:**
> I've identified several conditions related to root rot. Notable markers include yellowing leaves and mushy stems. I can provide the recommended treatment and prevention steps for these issues.


## ❓ FAQ

**Q: How do I find my Perenual API Key?**
Register for a free or paid account at [**perenual.com/docs/api**](https://perenual.com/docs/api), and you will find your API Key in your dashboard. Copy and paste it below.

**Q: Does it support disease identification?**
Yes. The `search_plant_diseases` tool allows your agent to audit common pests and diseases and retrieve recommended solutions.

**Q: Are care guides included for all species?**
Yes. The `get_plant_care_guide` tool retrieves specific maintenance instructions including watering frequency and sunlight exposure for most species.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perenual-plant-api](https://vinkius.com/mcp/perenual-plant-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perenual Plant API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `perenual-plant-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perenual Plant API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perenual-plant-api": {
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
