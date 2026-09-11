# Long-Term Mine Plan Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/long-term-mine-plan-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Generates life-of-mine schedules and resource depletion profiles.

## Description
This MCP server provides specialized tools for mining engineering. It allows AI agents to validate resource integrity using `analyze_resource_reserves`, create extraction roadmaps with `generate_production_schedule`, track inventory via `calculate_depletion_profile`, and identify operational bottlenecks with `evaluate_capacity_constraints`.


## Available Tools (4)
- **calculate_depletion_profile**: Tracks the remaining inventory of resources over the planned duration
- **analyze_resource_reserves**: Validates the integrity of the input data before planning begins
- **evaluate_capacity_constraints**: Identifies bottlenecks where the mine plan exceeds physical limits
- **generate_production_schedule**: Calculates the yearly movement of material based on constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Long-Term Mine Plan Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate if my reserve statement is consistent with my resource model data."

**🤖 AI Agent:**
> The resource validation is successful. The total ore tonnage is 5,000,000 and the reserve-to-resource ratio is 0.85.

---

**👤 You:**
> "Generate a production schedule for a mine with 2,000,000 tons of ore and a 500,000 ton annual capacity."

**🤖 AI Agent:**
> The production schedule is complete. The mine will operate for 4 years, extracting 500,000 tons of ore annually.

---

**👤 You:**
> "Check for capacity bottlenecks in my current mine plan."

**🤖 AI Agent:**
> No bottlenecks were detected. The planned ore and waste tonnage remain within the specified capacity limits for all years.


## ❓ FAQ

**Q: How do I validate my resource and reserve data?**
You can use the `analyze_resource_reserves` tool to ensure your reserve statement is consistent with your resource model.

**Q: Can I identify production bottlenecks?**
Yes, the `evaluate_capacity_constraints` tool identifies years where the plan exceeds processing or waste capacity limits.

**Q: How is the life-of-mine schedule generated?**
The `generate_production_schedule` tool calculates yearly material movement based on your processing capacity and mining sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/long-term-mine-plan-engine](https://vinkius.com/en/ai-agent-connect/long-term-mine-plan-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Long-Term Mine Plan Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `long-term-mine-plan-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Long-Term Mine Plan Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "long-term-mine-plan-engine": {
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
