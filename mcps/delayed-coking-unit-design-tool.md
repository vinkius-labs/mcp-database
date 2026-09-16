# Delayed Coking Unit Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/delayed-coking-unit-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design delayed coking units by calculating yields, drum dimensions, and operational schedules.

## Description
This MCP server provides specialized engineering tools for designing Delayed Coking Units (DCU). It allows users to determine product mass distribution using `calculate_yields`, calculate necessary drum sizes with `design_drum_geometry`, create operational timelines via `generate_cycle_schedule`, and evaluate operational hazards using `assess_coke_risk`. It is designed to help engineers manage residue conversion and mitigate shot coke risks.


## Available Tools (4)
- **calculate_yields**: Determines the expected mass distribution of products from a specific residue feed
- **design_drum_geometry**: Calculates the required physical dimensions for the coking drums
- **generate_cycle_schedule**: Provides the operational timeline for a multi-drum DCU setup
- **assess_coke_risk**: Evaluates the likelihood of producing shot coke and the resulting quality profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delayed Coking Unit Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the expected yields for a residue with density 0.95, viscosity 15, and sulfur 2.5 at 490 degrees Celsius?"

**🤖 AI Agent:**
> The expected yields are: coke yield of 45%, naphtha of 20%, gas oil of 25%, and diesel of 10%.

---

**👤 You:**
> "Calculate the drum dimensions for a feed rate of 500 tons per day with a 0.4 coke yield and a 12-hour cycle time."

**🤖 AI Agent:**
> The required drum dimensions are a diameter of 4.5 meters and a height of 12.0 meters, providing a total volume of 765 cubic meters.

---

**👤 You:**
> "Is there a high risk of shot coke if I use a residue with density 1.05 at 510 degrees Celsius?"

**🤖 AI Agent:**
> Yes, the risk level is High, and there is a significant operational risk due to the high density and temperature combination.


## ❓ FAQ

**Q: How do I calculate the expected liquid product yields?**
You can use the `calculate_yields` tool by providing the residue properties (density, viscosity, sulfur content) and the target coking temperature.

**Q: Can this tool help prevent shot coke production?**
Yes, the `assess_coke_risk` tool evaluates the likelihood of shot coke production based on residue density and temperature, helping to identify operational risks.

**Q: How are drum dimensions determined?**
The `design_drum_geometry` tool calculates the required diameter and height based on the daily feed rate, coke yield, and the desired safety factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/delayed-coking-unit-design-tool](https://vinkius.com/en/ai-agent-connect/delayed-coking-unit-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delayed Coking Unit Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `delayed-coking-unit-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delayed Coking Unit Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delayed-coking-unit-design-tool": {
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
