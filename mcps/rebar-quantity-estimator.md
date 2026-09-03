# Rebar Quantity Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rebar-quantity-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise rebar weights, lengths, and counts for structural elements.

## Description
This MCP server provides specialized tools for structural engineering reinforcement calculations. It allows AI agents to determine the exact quantity of longitudinal reinforcement and transverse stirrups for elements like beams, columns, and slabs. By using `estimate_total_project_rebar`, you can obtain a complete summary of total weight and length, accounting for concrete cover, lap lengths, and waste factors.


## Available Tools (4)
- **calculate_longitudinal_reinforcement**: Calculates the quantity of primary bars running the length of the element
- **calculate_transverse_reinforcement**: Calculates the quantity of stirrups or ties for the element
- **estimate_total_project_rebar**: Provides a high-level summary of all reinforcement for a single structural element
- **get_element_type_details**: Provides the standard reinforcement characteristics for a specific element type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebar Quantity Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the total rebar needed for a beam that is 5m long, 0.3m wide, and 0.5m high. Use 16mm longitudinal bars at 15cm spacing and 8mm stirrups at 20cm spacing, with 30mm concrete cover."

**🤖 AI Agent:**
> The total estimated rebar weight for the beam is 142.5 kg, with a total length of 32.4 meters.

---

**👤 You:**
> "How many longitudinal bars are needed for a 4m long column, 0.4m wide and 0.4m deep, using 20mm bars spaced at 10cm with 40mm cover?"

**🤖 AI Agent:**
> You will need 4 longitudinal bars for this column.

---

**👤 You:**
> "What are the standard reinforcement characteristics for a slab?"

**🤖 AI Agent:**
> For a slab, the standard lap factor is 1.2 and the standard stirrup spacing factor is 0.0.


## ❓ FAQ

**Q: What structural elements are supported?**
The server supports standard elements including beams, columns, slabs, and footings via the `get_element_type_details` tool.

**Q: How is the total weight calculated?**
Total weight is calculated by determining the effective length of bars (subtracting concrete cover), adding required lap lengths, and applying the steel density constant.

**Q: Can I include a waste factor in my estimate?**
Yes, all calculation tools allow for an optional `wasteFactor` to account for cutting losses and site handling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rebar-quantity-estimator](https://vinkius.com/ai-agent-connect/rebar-quantity-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebar Quantity Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rebar-quantity-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebar Quantity Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebar-quantity-estimator": {
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
