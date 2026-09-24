# Meal Per Diem Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meal-per-diem-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates travel meal allowances based on daily rates and trip duration.

## Description
This MCP server provides tools to automate travel reimbursement calculations. It allows AI agents to determine total meal allowances using `calculate_total_allowance`, verify trip durations with `validate_travel_days`, look up standardized rates via `get_rate_tier_info`, and generate cost reports with `summarize_trip_cost`.


## Available Tools (4)
- **calculate_total_allowance**: Calculates the total meal allowance for a specific trip
- **get_rate_tier_info**: Retrieves the standardized daily rate based on a specific tier of travel
- **summarize_trip_cost**: Provides a detailed breakdown of a trip's meal cost for reporting
- **validate_travel_days**: Verifies if a provided number of travel days is within acceptable business bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meal Per Diem Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total allowance for a 5-day trip with a daily rate of 50."

**🤖 AI Agent:**
> The total meal allowance for a 5-day trip at a rate of 50 per day is 250.

---

**👤 You:**
> "What is the daily rate for the Premium Tier?"

**🤖 AI Agent:**
> The daily rate for the Premium Tier is 75.

---

**👤 You:**
> "Provide a cost summary for a 3-day trip at 40 per day."

**🤖 AI Agent:**
> Daily Rate: 40, Travel Days: 3, Total Allowance: 120.


## ❓ FAQ

**Q: How do I calculate the total allowance for a trip?**
You can use the `calculate_total_allowance` tool by providing the daily meal rate and the total number of travel days.

**Q: Can I check if a trip duration is valid?**
Yes, the `validate_travel_days` tool checks if the number of days meets standard business travel policies.

**Q: How can I find the rate for a specific travel tier?**
Use the `get_rate_tier_info` tool with the specific tier identifier to retrieve the daily rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meal-per-diem-calculator](https://vinkius.com/en/ai-agent-connect/meal-per-diem-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meal Per Diem Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meal-per-diem-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meal Per Diem Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meal-per-diem-calculator": {
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
