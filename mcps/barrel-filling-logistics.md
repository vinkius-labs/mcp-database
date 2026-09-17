# Barrel Filling Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/barrel-filling-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Plan wine distribution, barrel selection, and cellar filling schedules.

## Description
This MCP server provides tools to manage the complex logistics of wine barrel filling. It allows for calculating the exact resources needed via `calculate_filling_requirements`, selecting optimal containers with `optimize_barrel_selection` to maintain lot segregation, and generating actionable work plans with `generate_filling_schedule`. It also includes `validate_cellar_capacity` to ensure all planned operations respect the physical constraints of the cellar layout.


## Available Tools (4)
- **calculate_filling_requirements**: Determines the fundamental resources needed to execute a filling plan
- **generate_filling_schedule**: Creates a time-based plan for the cellar staff to perform the filling operations
- **optimize_barrel_selection**: Selects the most appropriate barrels from inventory to satisfy the wine volume requirement while respecting lot segregation
- **validate_cellar_capacity**: Validates if the current cellar layout can accommodate the planned wine volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Barrel Filling Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many barrels do I need for 5000 liters of wine at 95% fill?"

**🤖 AI Agent:**
> You will need 11 barrels to accommodate 5000 liters at a 95% fill level.

---

**👤 You:**
> "Find the best barrels for 2000 liters of wine, preferring barrels that are 5 years old."

**🤖 AI Agent:**
> The system has selected 4 barrels with an age of 5 years, providing a total capacity of 2100 liters.

---

**👤 You:**
> "Create a filling schedule for these barrel IDs: B001, B002, B003 with a daily capacity of 500 liters."

**🤖 AI Agent:**
> The filling operation will take 2 days. Day 1: B001 and B002. Day 2: B003.


## ❓ FAQ

**Q: How do I know how many barrels I need?**
You can use the `calculate_filling_requirements` tool by providing the total wine volume and your target fill percentage.

**Q: Can I prioritize specific barrel ages?**
Yes, the `optimize_barrel_selection` tool allows you to specify a preferred barrel age to help with lot segregation.

**Q: How can I ensure my plan fits in the cellar?**
Use the `validate_cellar_capacity` tool to check if your proposed volume exceeds the capacity of a specific cellar zone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/barrel-filling-logistics](https://vinkius.com/en/ai-agent-connect/barrel-filling-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Barrel Filling Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `barrel-filling-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Barrel Filling Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "barrel-filling-logistics": {
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
