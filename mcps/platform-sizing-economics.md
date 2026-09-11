# Platform Sizing & Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/platform-sizing-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize offshore platform selection and physical dimensions based on production and environment.

## Description
This MCP server provides specialized tools for offshore engineering economics. It allows users to determine the most efficient platform type using `get_optimal_configuration`, calculate physical footprints with `estimate_deck_dimensions`, perform full lifecycle cost analysis via `calculate_lifecycle_costs`, and assess environmental risks through `analyze_metocean_impact`. It balances production profiles against CAPEX, water depth, and metocean conditions to guide structural decisions.


## Available Tools (4)
- **analyze_metocean_impact**: Evaluates how environmental conditions will drive up the structural weight and costs
- **calculate_lifecycle_costs**: Provides a full economic breakdown of the platform's total investment lifecycle
- **estimate_deck_dimensions**: Calculates the physical footprint and deck area needed to support the production equipment
- **get_optimal_configuration**: Determines the most economically efficient platform type based on environment and production needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Platform Sizing & Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best platform type for a site with 500m water depth and 50,000 annual production at medium metocean severity?"

**🤖 AI Agent:**
> The optimal configuration for these conditions is a floating platform.

---

**👤 You:**
> "Calculate the deck area for a fixed platform with 20,000 annual production and 5 wells."

**🤖 AI Agent:**
> The required deck area is 4,500 square meters with a topside weight capacity of 2,500 tonnes.

---

**👤 You:**
> "What are the lifecycle costs for a floating platform with 3,000 tonnes topside weight at 400m depth?"

**🤖 AI Agent:**
> The total CAPEX is $450,000,000, consisting of $250,000,000 for fabrication, $150,000,000 for installation, and $50,000,000 for decommissioning.


## ❓ FAQ

**Q: How do I find the best platform for my site?**
You can use the `get_optimal_configuration` tool, providing the water depth, expected annual production, and metocean severity.

**Q: Can I calculate the total cost of the project?**
Yes, the `calculate_lifecycle_costs` tool provides a breakdown of fabrication, installation, and decommissioning costs.

**Q: How does environmental severity affect my design?**
The `analyze_metocean_impact` tool evaluates how waves and wind increase structural weight and risk factors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/platform-sizing-economics](https://vinkius.com/en/ai-agent-connect/platform-sizing-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Platform Sizing & Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `platform-sizing-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Platform Sizing & Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "platform-sizing-economics": {
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
