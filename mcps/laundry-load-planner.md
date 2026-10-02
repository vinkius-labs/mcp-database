# Laundry Load Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/laundry-load-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan efficient laundry cycles by managing garment weights, machine capacities, and time constraints.

## Description
The Laundry Load Planner connects AI agents to your laundry management logic. It calculates optimal wash and dry cycles by respecting machine capacities and garment-specific requirements. Use `generate_full_schedule` to create a complete, time-ordered plan that fits within your available hours, or use `calculate_wash_plan` and `calculate_dry_plan` to analyze specific stages of the process. This tool ensures that weight limits for washers and dryers are never exceeded and that all tasks are completed within your time window.


## Available Tools (4)
- **calculate_dry_plan**: Determines how many drying cycles are required based on the results of the wash plan
- **calculate_wash_plan**: Determines how many wash loads are required to process all garments
- **generate_full_schedule**: Produces a complete, time-ordered plan for all laundry tasks
- **get_garment_requirements**: g., whites, colors, delicates).

Retrieves the necessary wash and dry parameters for a specific category of clothing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laundry Load Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan my laundry: I have 5kg of whites and 3kg of colors. My washer capacity is 4kg and my dryer capacity is 5kg. I have 4 hours available."

**🤖 AI Agent:**
> The laundry plan is complete. You will need 2 wash loads (one for whites, one for colors) and 2 drying cycles. The total time required is 3.5 hours, which fits within your 4-hour window.

---

**👤 You:**
> "What are the requirements for the 'delicates' category?"

**🤖 AI Agent:**
> The 'delicates' category requires a wash temperature of 30°C, a wash duration of 30 minutes, and a drying duration of 45 minutes.

---

**👤 You:**
> "Calculate the wash plan for 10kg of towels with a 6kg washer capacity."

**🤖 AI Agent:**
> To process 10kg of towels with a 6kg capacity, 2 wash loads are required. Each load will handle 5kg.


## ❓ FAQ

**Q: How do I create a complete laundry schedule?**
You can use the `generate_full_schedule` tool. Provide the list of garments with their weights, the washer and dryer capacities, and the total hours you have available.

**Q: Can I mix different garment categories in one load?**
No. To ensure wash requirements like temperature are met, garments of different categories cannot be mixed in the same wash load.

**Q: What happens if my laundry exceeds the machine capacity?**
The tool will automatically split the garments into multiple sequential loads to ensure no single load exceeds the washer or dryer capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/laundry-load-planner](https://vinkius.com/en/ai-agent-connect/laundry-load-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laundry Load Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `laundry-load-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laundry Load Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laundry-load-planner": {
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
