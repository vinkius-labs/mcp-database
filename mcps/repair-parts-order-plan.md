# Repair Parts Order Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-parts-order-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Sequences part procurement based on diagnostic requirements and supplier lead times.

## Description
This MCP server provides logistical orchestration for repair workflows. It uses tools like `get_procurement_sequence` to create optimal ordering schedules, `validate_budget_compliance` to ensure financial constraints are met, and `check_supplier_lead_times` to verify that all components arrive before the scheduled appointment. It also includes `calculate_contingency_options` to identify backup suppliers when primary choices fail availability or timing requirements.


## Available Tools (4)
- **calculate_contingency_options**: Identifies alternative parts or suppliers when the primary selection is unavailable or too slow
- **check_supplier_lead_times**: Verifies the feasibility of arrival dates for all selected suppliers
- **get_procurement_sequence**: Generates the optimal chronological list of parts to order to meet the repair deadline
- **validate_budget_compliance**: Checks if the proposed parts order stays within the allocated financial limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Parts Order Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a procurement sequence for these parts: [{"partId": "P1"}, {"partId": "P2"}] with supplier data [{"partId": "P1", "supplierId": "S1", "leadTime": 5}] and an appointment date of 2025-05-20."

**🤖 AI Agent:**
> The optimal sequence is to order part P1 on 2025-05-15 to ensure arrival by 2025-05-20.

---

**👤 You:**
> "Check if this order is within a $500 budget: [{"partId": "P1", "price": 250}, {"partId": "P2", "price": 200}]."

**🤖 AI Agent:**
> The total cost is $450, which is within the $500 budget. You have $50 remaining.

---

**👤 You:**
> "Verify if all parts will arrive before the appointment on 2025-06-01 for the following orders: [{"partId": "P1", "expectedArrivalDate": "2025-05-30"}]."

**🤖 AI Agent:**
> All parts are on time. Part P1 is expected to arrive on 2025-05-30, which is before the appointment.


## ❓ FAQ

**Q: How does the tool determine the order of parts?**
The `get_procurement_sequence` tool prioritizes parts based on their lead times relative to the appointment date, ensuring critical path items are ordered first.

**Q: Can I check if my repair plan stays within budget?**
Yes, you can use `validate_budget_compliance` to verify that the total cost of all proposed part orders does not exceed your allocated budget.

**Q: What happens if a primary supplier is out of stock?**
You can use `calculate_contingency_options` to find alternative suppliers or parts that still meet the required lead time and budget constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-parts-order-plan](https://vinkius.com/en/ai-agent-connect/repair-parts-order-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Parts Order Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-parts-order-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Parts Order Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-parts-order-plan": {
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
