# NoiseMeters API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noisemeters-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-research](../categories/scientific-research.md)

Monitor noise levels — audit decibels and instruments via AI.

## Description
Empower your AI agent to orchestrate your entire acoustic research and noise auditing workflow with the **NoiseMeters API**, the specialized source for high-resolution environmental sound data. By connecting the NoiseMeters API to your agent, you transform complex decibel searches into a natural conversation. Your agent can instantly retrieve real-time noise levels, audit historical measurements, and query instrument health without you ever touching a technical portal. Whether you are conducting industrial compliance research or monitoring urban noise constraints, your agent acts as a real-time acoustic consultant, ensuring your data is always verified and precise.

### What you can do

- **Acoustic Auditing** — Retrieve real-time decibel (dB) levels for any registered instrument and maintain a clear view of environmental noise.
- **Measurement Oversight** — Audit historical noise measurements to understand the temporal distribution of sound intensity instantly.
- **Instrument Discovery** — List all registered monitoring instruments in your catalog to maintain strict organizational control over regional data.
- **Operational Monitoring** — Check API status to ensure your acoustic research workflow is always operational.
- **Environmental Intelligence** — Retrieve detailed metadata for specific instruments to assist in deep-dive sound classification.

### How it works

1. Subscribe to this server
2. Enter your NoiseMeters API Key
3. Start managing your acoustic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Engineers** — monitor noise compliance and retrieve official metadata straight from your workflow.
- **Occupational Health Leads** — verify worker exposure and audit noise patterns without manual searching.
- **Urban Planners** — perform rapid audits of city sound levels and identify relevant acoustic markers through natural language.
- **Operations Leads** — automate acoustic data querying to orchestrate cross-functional safety teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the NoiseMeters service is operational
- **get_live_noise_data**: Get the most recent real-time noise level from an instrument
- **get_noise_measurements**: Get historical noise measurements for a specific instrument
- **list_noise_instruments**: List all noise monitoring instruments registered in your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NoiseMeters API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get live noise data for instrument 'INS-12345' using NoiseMeters."

**🤖 AI Agent:**
> I've retrieved the live noise data for instrument INS-12345! The current level is identified as 65.2 dB. Would you like the historical measurement metadata or the location details for this site?

---

**👤 You:**
> "List all my noise monitoring instruments."

**🤖 AI Agent:**
> I've retrieved your instrument catalog from NoiseMeters! You have 3 active devices, including 'Factory-South' and 'Site-Alpha'. I can provide the real-time decibel metadata for any of these instruments.

---

**👤 You:**
> "Show noise measurements for 'INS-67890' starting from '2024-05-01'."

**🤖 AI Agent:**
> I've identified the measurements for that instrument! There were 24 entries recorded since May 1st. I can assist you with an audit of the peak sound intensity and duration markers if you'd like.


## ❓ FAQ

**Q: How do I find my NoiseMeters API Key?**
Log in to your [**NoiseMeters dashboard**](https://api.noisemeters.com/), and you will find your API Key under your account or integrations section. Copy and paste it below.

**Q: Does it support real-time sound levels?**
Yes. The `get_live_noise_data` tool provides the most recent decibel measurement received from the specified instrument ID.

**Q: Can the agent list my monitoring instruments?**
Yes. The `list_noise_instruments` tool retrieves all noise monitoring devices registered in your account with their unique identifiers and names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noisemeters-api](https://vinkius.com/mcp/noisemeters-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NoiseMeters API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `noisemeters-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NoiseMeters API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noisemeters-api": {
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
