# Produced Water Treatment Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/produced-water-treatment-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design and size oil-water separation systems including API separators, flotation cells, and filtration units.

## Description
This MCP server provides specialized engineering tools for designing produced water treatment systems in oil and gas operations. It allows engineers to calculate the physical dimensions of an API separator using `get_separator_sizing`, determine the necessary surface area for flotation units with `get_flotation_dimensions`, and select an optimal sequence of equipment via `get_treatment_train_selection`. Additionally, it can calculate tertiary polishing needs using `get_filtration_requirements`. The tools account for dispersed oil removal and help meet strict environmental discharge or reservoir reinjection specifications.


## Available Tools (4)
- **get_filtration_requirements**: Determines the filter media type and surface area required for tertiary polishing
- **get_flotation_dimensions**: Calculates the surface area and volume needed for a flotation cell
- **get_separator_sizing**: Determines the required physical dimensions of an API-style gravity separator
- **get_treatment_train_selection**: Recommends a specific sequence of equipment (a "train") to meet a final specification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Produced Water Treatment Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What size API separator do I need for a flow rate of 500 m3/h with 1000 ppm oil in water, aiming for 50 ppm?"

**🤖 AI Agent:**
> The required API separator would have a vessel diameter of 3.5 meters and a length of 12 meters, providing a residence time of 15 minutes.

---

**👤 You:**
> "Recommend a treatment train for 100 m3/h of water starting at 2000 ppm oil for reinjection."

**🤖 AI Agent:**
> The recommended treatment train is: API Separator followed by a Flotation cell and a final Filtration step.

---

**👤 You:**
> "Calculate flotation cell dimensions for 250 m3/h with 500 ppm oil in water and a target of 20 ppm."

**🤖 AI Agent:**
> The flotation cell requires a surface area of 45 square meters and a cell volume of 90 cubic meters.


## ❓ FAQ

**Q: How do I size a gravity separator?**
You can use the `get_separator_sizing` tool by providing the flow rate, the initial oil concentration, and your target oil concentration.

**Q: Can this tool help select a full treatment sequence?**
Yes, the `get_treatment_train_selection` tool recommends a specific sequence of equipment to meet your final discharge or reinjection requirements.

**Q: Does it support reinjection specifications?**
Yes, the tools account for the stricter requirements often needed for reservoir reinjection versus environmental discharge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/produced-water-treatment-designer](https://vinkius.com/en/ai-agent-connect/produced-water-treatment-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Produced Water Treatment Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `produced-water-treatment-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Produced Water Treatment Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "produced-water-treatment-designer": {
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
