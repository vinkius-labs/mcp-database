# Cooking Session Timeline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cooking-session-timeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synchronize prep, cooking, and resting stages for multiple dishes into a single optimized plan.

## Description
This MCP server acts as a culinary synchronization engine. It manages the complex timing required to prepare multiple dishes simultaneously, ensuring that prep work, active cooking, and critical resting periods are perfectly sequenced. By accounting for resource constraints like oven temperature limits and burner availability, it generates a master schedule that ensures all components reach their ideal serving time together. Use `calculate_timeline` to generate a full schedule, `optimize_prep_work` to balance your workload, and `validate_resource_conflict` to ensure your plan is feasible.


## Available Tools (4)
- **calculate_timeline**: Generates a synchronized master schedule for a set of dishes
- **get_dish_templates**: Retrieves a list of pre-defined dish templates to use as a basis for planning
- **optimize_prep_work**: Reorders non-cooking tasks (Prep) to minimize idle time or maximize efficiency
- **validate_resource_conflict**: Checks if a proposed sequence of tasks violates hardware constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cooking Session Timeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a cooking timeline for a Roast Beef and Mashed Potatoes to be served at 7:00 PM. My oven goes up to 250°C and I have 4 burners."

**🤖 AI Agent:**
> 6:00 PM: Start Prep for Roast Beef. 6:30 PM: Roast Beef enters oven at 190°C. 6:45 PM: Prep Mashed Potatoes. 7:00 PM: Roast Beef finishes cooking and begins resting. 7:05 PM: Serve Roast Beef and Mashed Potatoes.

---

**👤 You:**
> "Check if this plan is feasible: Roast Beef on burner at 6:00 PM and Salmon on burner at 6:00 PM, but I only have 1 burner."

**🤖 AI Agent:**
> No, the plan is not feasible. There is a conflict: two dishes are assigned to a burner at 6:00 PM, but only 1 burner is available.

---

**👤 You:**
> "What dish templates are available for proteins?"

**🤖 AI Agent:**
> Available protein templates include Roast Beef and Salmon.


## ❓ FAQ

**Q: How does the tool handle oven constraints?**
The `calculate_timeline` tool checks your specified `ovenTemperatureLimit`. If a dish requires a temperature higher than your oven can reach, the calculation will fail to prevent invalid plans.

**Q: Can I optimize my preparation time?**
Yes, you can use `optimize_prep_work` to reorder preparation tasks. You can choose between 'minimumDuration' for the fastest finish or 'balancedLoad' to spread out the work.

**Q: How are stovetop burners managed?**
You specify your `burnerCount` during timeline generation. The engine ensures that the number of dishes using a burner at any single timestamp never exceeds your available capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cooking-session-timeline](https://vinkius.com/en/ai-agent-connect/cooking-session-timeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cooking Session Timeline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cooking-session-timeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cooking Session Timeline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cooking-session-timeline": {
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
