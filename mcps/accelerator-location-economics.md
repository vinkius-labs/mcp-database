# Accelerator Location Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-location-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze and compare geographic locations for accelerator programs using cost and ecosystem metrics.

## Description
This MCP server provides analytical tools for accelerator operators to evaluate potential geographic sites. It balances financial overhead against qualitative advantages like talent availability and ecosystem maturity. Use `get_location_comparison` to rank multiple sites, `get_ecosystem_analysis` for deep dives into specific location profiles, and `get_cost_breakdown` to calculate net operating costs after government incentives.


## Available Tools (3)
- **get_cost_breakdown**: Details the financial impact of choosing a specific location, focusing on the net cost after incentives
- **get_ecosystem_analysis**: Provides a deep dive into the qualitative strengths and talent profile of a single specific location
- **get_location_comparison**: Compares multiple potential locations to identify the most viable site based on cost and ecosystem value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Location Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare Austin, Berlin, and Singapore with rent costs of 500k, 400k, and 600k respectively, talent scores of 0.8, 0.7, and 0.9, ecosystem strengths of 0.7, 0.6, and 0.8, and incentives of 50k, 30k, and 100k."

**🤖 AI Agent:**
> Singapore is the recommended location with an ecosystem score of 0.72 and a total operating cost of $500,000.

---

**👤 You:**
> "What is the ecosystem maturity for a location with an ecosystem strength of 0.4 and talent availability of 0.5?"

**🤖 AI Agent:**
> The location has a maturity tier of 'Developing'.

---

**👤 You:**
> "Calculate the net cost for a location with $200,000 rent and $40,000 in government incentives."

**🤖 AI Agent:**
> The net operating cost is $160,000 with an incentive impact ratio of 0.2.


## ❓ FAQ

**Q: How is the ecosystem score calculated?**
The ecosystem score is the product of talent availability and ecosystem strength.

**Q: What determines if a location is recommended?**
A location is recommended if its ecosystem score divided by its total operating cost is higher than the average ratio across all evaluated locations.

**Q: Can I compare multiple cities at once?**
Yes, you can use `get_location_comparison` to evaluate multiple locations simultaneously based on rent, talent, and incentives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-location-economics](https://vinkius.com/ai-agent-connect/accelerator-location-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Location Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-location-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Location Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-location-economics": {
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
