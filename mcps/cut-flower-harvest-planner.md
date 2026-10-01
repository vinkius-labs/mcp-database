# Cut Flower Harvest Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cut-flower-harvest-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Precision planning for stem requirements, harvest scheduling, and yield projections.

## Description
This MCP connects AI agents to precision agricultural planning tools. It allows for calculating exact stem demand from bouquet orders using `calculate_stem_demand`, projecting usable yields with `project_effective_yield`, verifying harvest feasibility with `validate_harvest_feasibility`, and mapping out optimal picking dates with `generate_harvest_schedule`.


## Available Tools (4)
- **calculate_stem_demand**: Determines the total number of individual stems required to fulfill a specific set of bouquet orders
- **generate_harvest_schedule**: Identifies the dates when harvesting must occur based on crop maturity and order deadlines
- **project_effective_yield**: Calculates how many usable stems will be available after accounting for natural crop loss
- **validate_harvest_feasibility**: Checks if the expected stem demand can be met by the projected crop yield for a specific harvest date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cut Flower Harvest Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many stems do I need for 5 bouquets that require 10 stems each?"

**🤖 AI Agent:**
> You need 50 stems in total.

---

**👤 You:**
> "If I have 1000 stems and a 10% loss rate, what is my effective yield?"

**🤖 AI Agent:**
> Your effective yield is 900 stems.

---

**👤 You:**
> "Is a harvest of 100 stems enough for 80 required stems with a 15% buffer?"

**🤖 AI Agent:**
> No, with a 15% buffer, you need 92 stems, so 100 stems is sufficient to meet the requirement.


## ❓ FAQ

**Q: How do I calculate the total stems needed for my orders?**
You can use the `calculate_stem_demand` tool by providing your bouquet orders and their stem definitions.

**Q: Can I account for crop loss in my planning?**
Yes, the `project_effective_yield` tool calculates usable stems after applying your expected loss rate.

**Q: How do I know if my harvest will meet demand?**
Use `validate_harvest_feasibility` to compare required stems against your projected yield, including an optional safety buffer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cut-flower-harvest-planner](https://vinkius.com/en/ai-agent-connect/cut-flower-harvest-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cut Flower Harvest Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cut-flower-harvest-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cut Flower Harvest Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cut-flower-harvest-planner": {
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
