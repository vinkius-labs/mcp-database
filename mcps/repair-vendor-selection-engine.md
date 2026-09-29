# Repair Vendor Selection Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-vendor-selection-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

A decision-support engine that evaluates and selects the optimal repair service provider based on user priorities.

## Description
This MCP server provides a sophisticated decision-support engine for selecting repair service providers. It connects AI agents to a multi-dimensional evaluation framework that synthesizes vendor qualifications, service areas, availability, and pricing. Using the `evaluate_vendor_scores` tool, agents can apply weighted user preferences to rank candidates. Once a decision is made, the `book_repair_service` tool facilitates the final transition from candidate to booked status. This bridge allows AI assistants to act as expert procurement agents for home and technical repairs.


## Available Tools (4)
- **book_repair_service**: Executes the booking of a repair service
- **evaluate_vendor_scores**: 0), and request details.

Calculates comparative scores for eligible vendors using user-defined weights
- **get_eligible_vendors**: g., electronics, appliance) and the geographic location.

Identifies vendors capable of performing the requested repair based on type and location
- **get_vendor_details**: Retrieves granular details for a specific vendor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Vendor Selection Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me an appliance repair technician in Chicago and tell me who is the best value based on price and warranty."

**🤖 AI Agent:**
> The best vendor for your appliance repair in Chicago is 'QuickFix Solutions'. They have a total score of 0.85, offering a competitive quote of $120 and a 12-month warranty.

---

**👤 You:**
> "What are the specific details and available slots for vendor ID 'v-992'?"

**🤖 AI Agent:**
> Vendor 'v-992' offers a quote of $85.00 with a 6-month warranty. Available slots are: 2024-10-15T10:00:00Z and 2024-10-16T14:00:00Z.

---

**👤 You:**
> "Book the repair with vendor 'v-101' for the slot 'slot-abc-123' for John Doe at john@example.com."

**🤖 AI Agent:**
> Booking confirmed! Your booking ID is BK-7721. The technician is scheduled to arrive on 2024-11-01 at 09:00 AM.


## ❓ FAQ

**Q: How does the engine decide which vendor is best?**
The engine uses the `evaluate_vendor_scores` tool to calculate a total score for each vendor. This score is derived by multiplying normalized vendor attributes (like price and warranty) by the specific weights assigned by the user.

**Q: Can I book a service directly through the AI?**
Yes. After identifying the best vendor, you can use the `book_repair_service` tool to commit to a specific time slot and finalize the booking.

**Q: How do I know if a vendor can service my area?**
You should first use the `get_eligible_vendors` tool. It filters the vendor registry by repair type and geographic location to ensure only capable providers are considered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-vendor-selection-engine](https://vinkius.com/en/ai-agent-connect/repair-vendor-selection-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Vendor Selection Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-vendor-selection-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Vendor Selection Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-vendor-selection-engine": {
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
