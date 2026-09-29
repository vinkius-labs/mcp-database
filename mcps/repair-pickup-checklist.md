# Repair Pickup Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-pickup-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Verify automotive or technical repairs against original work orders.

## Description
This MCP server provides a specialized toolset for service advisors and customers to ensure successful vehicle or device handovers. Use `get_pickup_checklist` to generate itemized lists for parts and accessories, `verify_repair_compliance` to check if installed parts match the original order, `check_financial_clearance` to confirm payment or warranty status, and `generate_discrepancy_report` to document any mismatches found during inspection.


## Available Tools (4)
- **check_financial_clearance**: Determines if the customer is cleared to take the item based on payment and warranty status
- **generate_discrepancy_report**: Creates a formal list of all mismatches found during the pickup process for service advisor review
- **get_pickup_checklist**: Generates a comprehensive, itemized checklist for a customer to walk through during the vehicle/device handover
- **verify_repair_compliance**: Compares the actual completed work against the original authorization to identify missing items or unauthorized additions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Pickup Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a pickup checklist for repair order RO-9928."

**🤖 AI Agent:**
> Here is your checklist for RO-9928: 
- Work Performed: Brake Pads (Installed), Rotor (Installed)
- Operational Integrity: Braking Smoothness (Confirmed)
- Physical Inventory: Floor Mats (Present)

---

**👤 You:**
> "Is repair order RO-5542 cleared for pickup?"

**🤖 AI Agent:**
> Yes, RO-5542 is cleared. The balance due is $0.00.

---

**👤 You:**
> "Check if the repair for RO-1122 is compliant with parts: Brake Pads, Brake Fluid."

**🤖 AI Agent:**
> The repair is compliant. All requested parts were installed and functions are verified.


## ❓ FAQ

**Q: How do I generate a checklist for a customer?**
You can use the `get_pickup_checklist` tool by providing the specific repair order ID.

**Q: Can I check if a repair is paid for?**
Yes, use `check_financial_clearance` to verify if the balance is zero or covered by warranty.

**Q: What happens if a part is missing?**
If a part is missing, use `verify_repair_compliance` to identify the mismatch and `generate_discrepancy_report` to document it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-pickup-checklist](https://vinkius.com/en/ai-agent-connect/repair-pickup-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Pickup Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-pickup-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Pickup Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-pickup-checklist": {
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
