# Slab Thickness Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slab-thickness-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Estimate minimum concrete slab thickness based on span and construction type.

## Description
This MCP server provides structural engineering pre-dimensioning tools for concrete slabs. Use `calculate_minimum_thickness` to determine the required depth for solid, ribbed, or precast slabs based on their span in meters. You can also use `check_analysis_requirement` to see if a specific span requires formal professional analysis, and `get_slab_metadata` to understand the complexity of different construction methods.


## Available Tools (4)
- **get_slab_metadata**: Retrieves metadata for a specific slab type
- **calculate_minimum_thickness**: Calculates the minimum thickness for a slab
- **check_analysis_requirement**: Checks if structural analysis is required
- **list_all_slab_types**: Lists all supported slab types and their metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slab Thickness Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum thickness for a 5 meter solid slab?"

**🤖 AI Agent:**
> The estimated minimum thickness for a 5 meter solid slab is 0.12 meters.

---

**👤 You:**
> "Does a 12 meter span require formal analysis?"

**🤖 AI Agent:**
> Yes, for a 12 meter span, the status is 'alert' and professional structural analysis is required.

---

**👤 You:**
> "Tell me about ribbed slabs."

**🤖 AI Agent:**
> Ribbed slabs consist of a top compression flange and longitudinal ribs, allowing for larger spans with reduced concrete weight.


## ❓ FAQ

**Q: How accurate are these thickness estimates?**
These values are preliminary pre-dimensioning estimates based on standard ratios. They do not replace formal structural calculations by a licensed engineer.

**Q: When should I seek professional analysis?**
Use the `check_analysis_requirement` tool. If it returns an 'alert' status, a formal structural engineer's report is mandatory.

**Q: What slab types are supported?**
The tool supports solid, ribbed, and precast slab construction methods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slab-thickness-estimator](https://vinkius.com/mcp/slab-thickness-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slab Thickness Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slab-thickness-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slab Thickness Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slab-thickness-estimator": {
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
