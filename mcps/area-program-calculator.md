# Area Program Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/area-program-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates minimum required total area for any project based on room functions and structural complexity.

## Description
Building a new structure requires more than just listing rooms. The biggest challenge is calculating the true minimum total programmatic area (TPA). Architects and developers often underestimate overhead, leading to costly redesigns or zoning violations.

The Area Program Calculator solves this by providing a precise estimate of required square footage. It works in three distinct stages: first, it uses `get_base_area_by_function` to establish the core usable area for each room based on its primary activity (e.g., sleeping, hygiene). Second, it applies structural overhead using `adjust_area_for_structure`, which calculates the necessary extra space for MEP systems and circulation hallways based on complexity (simple, medium, or high). Finally, it aggregates everything with `calculate_programmatic_needs` to return a single, reliable total programmatic area estimate. This process ensures your initial planning budget is accurate from day one.


## Available Tools
- **adjust_area_for_structure**: Adjust a base area for structural complexity overhead
- **get_base_area_by_function**: Get minimum usable area for an environment by its function type
- **calculate_programmatic_needs**: Calculate total programmatic area for all environments in a building program


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Area Program Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a plan for a small family home. It has 1 bedroom, 2 bathrooms, and a kitchenette. Use medium complexity."

**🤖 AI Agent:**
> The total estimated area is X sq meters. This was calculated by first finding the base areas using `get_base_area_by_function` for all components, then applying the 1.25 multiplier via `adjust_area_for_structure`, and finally summing it up with `calculate_programmatic_needs`.

---

**👤 You:**
> "Calculate the base area needed for a high-tech study room (StudyArea) that supports working functions. Use simple complexity first."

**🤖 AI Agent:**
> The minimum usable area is Y sq meters, as determined by `get_base_area_by_function`. If we apply the structural adjustment now using `adjust_area_for_structure` with 'simple', the total becomes Z sq meters.

---

**👤 You:**
> "Final check: Give me the total programmatic needs for 3 bedrooms, 2 bathrooms, and 1 livingroom, assuming high complexity."

**🤖 AI Agent:**
> The final required area is A sq meters. This result was derived by running all components through `calculate_programmatic_needs` with the 'high' structural standard applied consistently across the entire program.


## ❓ FAQ

**Q: What is the difference between base area and final adjusted area?**
The initial minimum usable space is found using `get_base_area_by_function`. The final, total required size includes structural overhead (hallways, utilities), which is calculated by the `adjust_area_for_structure` tool. Always use both for an accurate total.

**Q: Can I calculate the final area without listing all components?**
No. The `calculate_programmatic_needs` tool requires a complete list of environments, their functions, and component counts to ensure every required space is accounted for before giving a total area estimate.

**Q: What if my building structure changes from simple to high complexity?**
You must re-run the calculation using `adjust_area_for_structure` with the new 'high' complexity level. This change significantly increases the multiplier, accounting for major infrastructure shifts that affect the total program area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/area-program-calculator](https://vinkius.com/mcp/area-program-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Area Program Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `area-program-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Area Program Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "area-program-calculator": {
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
