# Loaner Item Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/loaner-item-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Manages loaner item reservations, availability, and return logistics.

## Description
This MCP server provides a specialized reservation engine for managing loaner equipment. It allows AI agents to `calculate_reservation_window` for repair periods, `check_item_availability` across different inventory tiers, `verify_insurance_compliance` for customers, and `generate_return_plan` to ensure timely equipment returns. It bridges the gap between repair schedules and logistical execution.


## Available Tools (4)
- **check_item_availability**: Confirm if a specific type of loaner item is available for the requested timeframe
- **generate_return_plan**: Create the logistics for returning the loaner item once the repair is complete
- **verify_insurance_compliance**: Check if a customer meets the necessary insurance criteria for a loaner item
- **calculate_reservation_window**: Determine if a loaner item can be reserved to cover a specific repair period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loaner Item Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a vehicle available from 2024-10-01 to 2024-10-05?"

**🤖 AI Agent:**
> Yes, there is 1 vehicle available for the requested period.

---

**👤 You:**
> "Calculate the reservation window for a 5-day repair starting on 2024-11-10."

**🤖 AI Agent:**
> The reservation window is confirmed from 2024-11-10 to 2024-11-15.

---

**👤 You:**
> "Check insurance for customer CUST-123 for a laptop category."

**🤖 AI Agent:**
> Customer CUST-123 is compliant with active coverage for the laptop category.


## ❓ FAQ

**Q: How do I check if a laptop is available for my repair window?**
You can use the `check_item_availability` tool by providing the item category (e.g., 'laptop') and the start and end dates of your required period.

**Q: Can I verify if a customer is eligible for a premium loaner?**
Yes, use the `verify_insurance_compliance` tool with the customer ID and the specific item category to confirm eligibility.

**Q: How do I know when the loaner item must be returned?**
Once a reservation is active, use `generate_return_plan` with the reservation ID to receive the return deadline and location details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/loaner-item-plan](https://vinkius.com/en/ai-agent-connect/loaner-item-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loaner Item Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `loaner-item-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loaner Item Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loaner-item-plan": {
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
