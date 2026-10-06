# Compostable Liner Use Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/compostable-liner-use-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate compostable liner requirements and costs for waste management services.

## Description
This MCP server provides specialized tools for waste management planning. It allows AI agents to determine the exact number of compostable liners needed per household and scale those requirements to entire communities. Using tools like `get_liner_requirement` and `calculate_pack_needs`, agents can accurately predict liner consumption based on bin volume, fill rates, and collection frequency. The server also handles financial modeling through `calculate_service_cost` and community-wide scaling via `get_community_impact` to provide a complete picture of operational needs and budget requirements.


## Available Tools (4)
- **calculate_pack_needs**: Calculates the number of full packs that must be purchased to satisfy the liner requirement
- **calculate_service_cost**: Determines the total financial cost for a specific quantity of packs
- **get_community_impact**: Scales individual liner and cost data to an entire community or service area
- **get_liner_requirement**: Determines how many individual compostable liners a single household will use over a specific period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Compostable Liner Use Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many liners does a household need if they have a 240L bin, a 75% fill rate, and 4 collections per month?"

**🤖 AI Agent:**
> A household with those parameters will require 4 liners per month.

---

**👤 You:**
> "If I need 120 liners and they come in packs of 50, how many packs should I buy?"

**🤖 AI Agent:**
> You will need to purchase 3 packs to cover the requirement.

---

**👤 You:**
> "What is the total cost for 5 packs if each pack costs $15.00?"

**🤖 AI Agent:**
> The total cost for 5 packs is $75.00.


## ❓ FAQ

**Q: How does the calculator determine liner needs?**
The `get_liner_requirement` tool calculates needs by assessing bin volume, the fill rate (percentage of capacity used), and how frequently the bin is emptied.

**Q: Can I calculate costs for an entire neighborhood?**
Yes, the `get_community_impact` tool scales individual household liner needs and costs to any number of households in a service area.

**Q: Does the tool account for commercial packaging?**
Yes, `calculate_pack_needs` converts the total number of individual liners required into the number of full commercial packs that must be purchased.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/compostable-liner-use-rate-calculator](https://vinkius.com/en/ai-agent-connect/compostable-liner-use-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Compostable Liner Use Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `compostable-liner-use-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Compostable Liner Use Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "compostable-liner-use-rate-calculator": {
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
