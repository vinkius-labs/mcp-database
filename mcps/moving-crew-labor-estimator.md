# Moving Crew Labor Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-crew-labor-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate moving labor hours, billable time, and total costs based on logistical variables.

## Description
This MCP server provides precise tools for moving companies to estimate labor requirements. Use `get_move_summary` to receive a complete breakdown of total labor hours, billable hours, and the final estimated charge. The server accounts for item complexity, floor levels, and elevator delays to ensure accurate man-hour calculations.


## Available Tools (4)
- **get_billable_hours**: Determines the final hours the client will be invoiced for
- **get_estimated_charge**: Calculates the final monetary cost of the moving service
- **get_labor_hours**: Calculates the total man-hours required for the move
- **get_move_summary**: Provides a complete breakdown of the labor, billing, and cost for a move


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Crew Labor Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the moving estimate for 5 hours of base tasks, 50 items, 3 floors, 10 minutes elevator delay per floor, a crew of 4, a minimum requirement of 10 hours, and an hourly rate of $150."

**🤖 AI Agent:**
> The total labor hours are 32.0, the billable hours are 32.0, and the estimated charge is $4,800.0.

---

**👤 You:**
> "What would the charge be for a move with 2 hours of tasks, 10 items, 1 floor, 0 elevator delay, 2 workers, a 5 hour minimum, and a $100 rate?"

**🤖 AI Agent:**
> The total labor hours are 4.0, the billable hours are 5.0, and the estimated charge is $500.0.

---

**👤 You:**
> "I need a summary for a large move: 10 hours task duration, 200 items, 5 floors, 15 minutes elevator delay, 6 workers, 20 hour minimum, and $120 hourly rate."

**🤖 AI Agent:**
> The total labor hours are 114.0, the billable hours are 114.0, and the estimated charge is $13,680.0.


## ❓ FAQ

**Q: How does the tool calculate total labor hours?**
The `get_labor_hours` tool calculates hours by combining base task duration with adjustments for item count, floor levels, and elevator delays, then scaling by the crew size.

**Q: What is the difference between labor hours and billable hours?**
Labor hours represent the actual work time calculated, while billable hours are the final amount charged, which is the greater of the calculated hours or the company's minimum requirement.

**Q: Can I get a full cost breakdown in one go?**
Yes, you can use `get_move_summary` to get the total labor hours, billable hours, and the estimated charge in a single response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-crew-labor-estimator](https://vinkius.com/en/ai-agent-connect/moving-crew-labor-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Crew Labor Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-crew-labor-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Crew Labor Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-crew-labor-estimator": {
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
