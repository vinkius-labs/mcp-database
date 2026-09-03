# Concrete Quantity Takeoff MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-quantity-takeoff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise concrete volumes for structural elements, accounting for openings and waste.

## Description
This MCP server provides specialized tools for construction professionals to determine exact concrete requirements. Use `calculate_element_volume` to compute gross and net volumes for slabs, columns, beams, and more, while accounting for structural openings. You can also use `estimate_pump_requirements` to calculate the extra volume needed for pump residue, or `compare_takeoff_scenarios` to evaluate how different waste factors impact your final order. The `validate_element_geometry` tool ensures your dimensions and voids are physically coherent before you place an order.


## Available Tools (4)
- **compare_takeoff_scenarios**: To evaluate how different waste factors or opening configurations impact the final order quantity
- **validate_element_geometry**: To check if the provided dimensions and openings are physically possible
- **calculate_element_volume**: To determine the net and gross volumes for a single structural element
- **estimate_pump_requirements**: To calculate the additional concrete volume required specifically due to the use of a concrete pump


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Quantity Takeoff** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the volume for a slab that is 10m by 5m with a thickness of 0.2m, including a 5% waste factor."

**🤖 AI Agent:**
> The total volume for the slab is 10.5 m³.

---

**👤 You:**
> "I have a net volume of 15 m³ and my pump waste factor is 0.03. How much extra concrete do I need?"

**🤖 AI Agent:**
> The pump waste volume is 0.45 m³, making the total required volume 15.45 m³.

---

**👤 You:**
> "Check if a column with dimensions 0.5m x 0.5m x 3m can have an opening of 0.6m x 0.6m."

**🤖 AI Agent:**
> The geometry is invalid because the opening dimensions exceed the element dimensions.


## ❓ FAQ

**Q: How does the tool handle openings in a structure?**
The `calculate_element_volume` tool subtracts the volume of all specified openings from the gross volume to provide an accurate net volume.

**Q: Can I account for concrete lost in a pump?**
Yes, use the `estimate_pump_requirements` tool to calculate the additional volume needed to cover residue left in the pump lines.

**Q: How can I compare different ordering strategies?**
You can use `compare_takeoff_scenarios` to see the difference in total volume between two different waste factors or configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-quantity-takeoff](https://vinkius.com/ai-agent-connect/concrete-quantity-takeoff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Quantity Takeoff** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-quantity-takeoff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Quantity Takeoff** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-quantity-takeoff": {
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
