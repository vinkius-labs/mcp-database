# Structural Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/structural-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Estimate structural engineering loads (permanent and variable) per square meter based on NBR 6120 standards.

## Description
The Structural Load Calculator is an essential tool for preliminary structural engineering assessments. It allows users to retrieve standardized load constants from the NBR 6120 standard and perform precise calculations for building components. Using `retrieve_load_constants`, you can find the permanent and variable loads for specific usage types like residential, commercial, garage, or rooftop. The `calculate_floor_load` tool enables detailed breakdown of loads for a single floor based on its area in square meters. Finally, `aggregate_foundation_lag` (via `aggregate_foundation_load`) allows you to sum all floor loads and apply a multiplier to estimate the total cumulative load transferred to the building's foundation.


## Available Tools (3)
- **calculate_floor_load**: Calculate total load for a single floor level
- **aggregate_foundation_load**: Aggregate total load for the entire building foundation
- **retrieve_load_constants**: ly: residential, commercial, garage, rooftop).

Retrieve NBR 6120 load constants for a specific usage type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Structural Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the permanent and variable load for a residential area?"

**🤖 AI Agent:**
> For a residential usage type, the permanent load is 400 kg/m² and the variable load is 150 kg/m².

---

**👤 You:**
> "Calculate the total load for a 200 square meter commercial floor."

**🤖 AI Agent:**
> For a 200 m² commercial area, the total floor load is 120,000 kg (80,000 kg permanent and 40,000 kg variable).

---

**👤 You:**
> "Estimate the foundation load for a building with two floors: one residential (100m²) and one garage (150m²)."

**🤖 AI Agent:**
> The cumulative building load is 122,500 kg. With a standard foundation self-weight multiplier of 1.0, the estimated total load on the foundation is 122,500 kg.


## ❓ FAQ

**Q: What standards does this calculator use?**
The calculator uses the hardcoded load constants derived from the NBR 6120 standard for various usage types.

**Q: How do I calculate the total load for a building?**
First, use `calculate_floor_load` for each floor level. Then, pass the resulting loads as a JSON array to the `aggregate_foundation_load` tool.

**Q: What usage types are supported?**
The supported usage types are residential, commercial, garage, and rooftop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/structural-load-calculator](https://vinkius.com/mcp/structural-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Structural Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `structural-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Structural Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "structural-load-calculator": {
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
