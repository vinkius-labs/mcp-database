# Mapflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Extract geospatial features from satellite imagery with AI that detects buildings, roads, and vegetation patterns automatically.

## Description
Connect your **Mapflow** account to any AI agent and manage geospatial AI processing through natural conversation.

### What you can do

- **Project Management** — Create and manage mapping projects
- **Image Processing** — Trigger AI models on satellite and drone imagery
- **Task Tracking** — Monitor processing status and completion
- **Dataset Browsing** — Access generated vector datasets and polygons
- **Model Management** — Browse available AI models (buildings, roads, forests)

### How it works

1. Subscribe to this server
2. Enter your Mapflow API Key
3. Start processing geospatial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GIS Specialists** — extract vector data from imagery automatically
- **Urban Planners** — map buildings and infrastructure
- **Environmentalists** — monitor forests and land use


## Available Tools (7)
- **create_processing**: Pass data as a JSON string.

Start a new imagery analysis
- **create_project**: Pass data as a JSON string.

Create a new project
- **get_processing_result**: Get processing result data
- **get_processing_status**: Check status of a processing job
- **list_models**: List available geospatial AI models
- **list_processings**: List all geospatial processings
- **list_projects**: List all MapFlow projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List available AI models and my active projects."

**🤖 AI Agent:**
> AI Models: 8 available. 'Building Footprints' (v2.1), 'Road Networks' (v1.5), 'Forest Cover' (v3.0), 'Construction Sites', 'Agriculture Fields'. Active projects: 3. 'Seattle Urban Planning' (Buildings), 'Amazon Monitoring' (Forest), 'Highway Survey' (Roads).

---

**👤 You:**
> "Start processing building footprints for the Seattle project."

**🤖 AI Agent:**
> Processing task started! ✅ Task ID: tsk_8901. Model: 'Building Footprints' (v2.1). Area: 14 sq km (Seattle downtown). Imagery: Maxar SecureWatch. Estimated time: 14 minutes. Status: Queued. Cost: 28 credits.

---

**👤 You:**
> "Check status of task tsk_8901 and show dataset results."

**🤖 AI Agent:**
> Task tsk_8901 status: Completed ✅ (Took 12m 45s). Dataset generated: 'Seattle_Buildings_Final'. Features extracted: 14,250 polygons. Confidence score avg: 92%. Formats available: GeoJSON, Shapefile, Geopackage. Ready for download.


## ❓ FAQ

**Q: Can I process satellite imagery and extract vector data?**
Yes. Trigger AI models on imagery to automatically extract buildings, roads, forests, and other features as vector polygons.

**Q: How does Mapflow authentication work?**
Mapflow uses Bearer authentication against `api.mapflow.ai/rest` using your API Key.

**Q: Can I track processing tasks?**
Yes. Monitor processing status, progress percentages, and access completion datasets when ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapflow](https://vinkius.com/mcp/mapflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mapflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mapflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapflow": {
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
