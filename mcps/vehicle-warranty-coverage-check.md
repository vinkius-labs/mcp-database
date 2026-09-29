# Vehicle Warranty Coverage Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vehicle-warranty-coverage-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Evaluates vehicle repair items against warranty terms, mileage limits, and exclusions.

## Description
This MCP server provides specialized diagnostic tools to determine if vehicle repairs are covered under a specific warranty. Use `check_repair_coverage` to evaluate a list of items against active policy rules, `validate_warranty_eligibility` to check if a vehicle is still within its general warranty window, `get_exclusion_summary` to isolate barred components, and `calculate_remaining_coverage` to find the remaining time and distance left in the policy.


## Available Tools (4)
- **calculate_remaining_coverage**: Calculates the remaining life of the warranty in both time and distance
- **check_repair_coverage**: Evaluates a list of repair items to determine if they are covered, excluded, or expired
- **get_exclusion_summary**: Provides a filtered list of items that are explicitly barred from coverage
- **validate_warranty_eligibility**: Determines if the vehicle is still under the general warranty umbrella


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vehicle Warranty Coverage Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my engine repair is covered. Current mileage is 45,000. Warranty started 2023-01-01, expires 2025-01-01, with a 50,000 mile limit. Exclusions: brake pads."

**🤖 AI Agent:**
> The engine repair is covered as it is within the time and mileage limits and is not on the exclusion list.

---

**👤 You:**
> "Is my vehicle still eligible for warranty? Current date is 2025-06-01, mileage is 55,000, limit is 50,000."

**🤖 AI Agent:**
> No, the vehicle is not eligible because the current mileage exceeds the allowed mileage limit.

---

**👤 You:**
> "How much warranty life is left? Started 2024-01-01, expires 2026-01-01, current mileage 10,000, limit 60,000."

**🤖 AI Agent:**
> You have 24 months and 50,000 miles of coverage remaining.


## ❓ FAQ

**Q: How do I check if a specific repair is covered?**
You can use the `check_repair_coverage` tool by providing the list of repair items, the current mileage, the warranty terms, and the list of exclusions.

**Q: Can I check how much mileage is left on my warranty?**
Yes, use the `calculate_remaining_coverage` tool to get the remaining months and miles based on your current mileage and the warranty limits.

**Q: What happens if a part is on the exclusion list?**
If a part is explicitly listed in the exclusions, it will be marked as excluded by the `check_repair_coverage` tool, regardless of the vehicle's mileage or age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vehicle-warranty-coverage-check](https://vinkius.com/en/ai-agent-connect/vehicle-warranty-coverage-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vehicle Warranty Coverage Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vehicle-warranty-coverage-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vehicle Warranty Coverage Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vehicle-warranty-coverage-check": {
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
